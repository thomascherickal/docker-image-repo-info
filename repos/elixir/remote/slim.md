## `elixir:slim`

```console
$ docker pull elixir@sha256:08cc5c5fef9f87ea61c0e9f653a48e4103aba9a24ac3519ddb30d923b269e615
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `elixir:slim` - linux; amd64

```console
$ docker pull elixir@sha256:fac67580d2a52d03ec67c63b420dce9bc39a3656d8ee085c07769a7b7c42d1d0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.2 MB (117179240 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e7595de6284c20a00fac5cbb2480558ebd0a34a243b8333ebccacc71334a55e`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:16 GMT
ADD file:89dfd7d3ed77fd5e05f20a0ab631142207ae462f5bbd877f8745d3930c751d87 in / 
# Wed, 22 Jul 2020 02:03:16 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 15:22:56 GMT
ENV OTP_VERSION=22.3.4.3
# Wed, 22 Jul 2020 15:22:56 GMT
LABEL org.opencontainers.image.version=22.3.4.3
# Wed, 22 Jul 2020 15:37:12 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="557376f7fef07fd7f08eedebcd23de8c921d7dfc9430e214d29a4726d92537d2" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 22 Jul 2020 15:37:13 GMT
CMD ["erl"]
# Thu, 23 Jul 2020 06:57:41 GMT
ENV ELIXIR_VERSION=v1.10.4 LANG=C.UTF-8
# Thu, 23 Jul 2020 06:59:06 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="8518c78f43fe36315dbe0d623823c2c1b7a025c114f3f4adbb48e04ef63f1d9f" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 06:59:06 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:31dd5ebca5efc5e96a425402fa85e492b02c8fe757dfd3edfdea2a7c67322909`  
		Last Modified: Wed, 22 Jul 2020 02:09:37 GMT  
		Size: 50.4 MB (50390325 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b4d5d9b542f49460d05c448a1f1fbab8a3181c15845cd2790ce50a9d6994602`  
		Last Modified: Wed, 22 Jul 2020 18:05:43 GMT  
		Size: 59.5 MB (59546143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9784ff76171ce66f369187d010ca6eef61830dd102b7c0eaaaec81e1a03b6628`  
		Last Modified: Thu, 23 Jul 2020 07:13:06 GMT  
		Size: 7.2 MB (7242772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; arm variant v7

```console
$ docker pull elixir@sha256:ab891bc0bb575eb4a9440998530ee3c3f9dea265271a91129438dcd2c89450bd
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.4 MB (108410918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bf10da5c2a5e48ce36243f5fa9455e33fa893346e91a16b3fb8d56c3a0eb491`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 22 Jul 2020 01:18:19 GMT
ADD file:38965defa0df84392a8ff562c2fa6393fe8d42f65f85591c07a581d694eebc30 in / 
# Wed, 22 Jul 2020 01:18:24 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 06:57:03 GMT
ENV OTP_VERSION=22.3.4.3
# Wed, 22 Jul 2020 06:57:08 GMT
LABEL org.opencontainers.image.version=22.3.4.3
# Wed, 22 Jul 2020 07:04:11 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="557376f7fef07fd7f08eedebcd23de8c921d7dfc9430e214d29a4726d92537d2" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 22 Jul 2020 07:04:17 GMT
CMD ["erl"]
# Thu, 23 Jul 2020 03:25:32 GMT
ENV ELIXIR_VERSION=v1.10.4 LANG=C.UTF-8
# Thu, 23 Jul 2020 03:28:11 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="8518c78f43fe36315dbe0d623823c2c1b7a025c114f3f4adbb48e04ef63f1d9f" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 03:28:12 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:f890282b0ef00faf11d62374bcdfc54ca574d085127c66977d9a08ab80978a98`  
		Last Modified: Wed, 22 Jul 2020 01:40:13 GMT  
		Size: 45.9 MB (45868714 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:025c8903bdac26224b76dd7ecae528c67d8035fcc5db602c7c9206584e2945ca`  
		Last Modified: Wed, 22 Jul 2020 08:31:36 GMT  
		Size: 55.3 MB (55299708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c9995e1424d1aa107ad781ac599e8b0ccbd91973293eb23b379a3905138fa532`  
		Last Modified: Thu, 23 Jul 2020 03:52:10 GMT  
		Size: 7.2 MB (7242496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; arm64 variant v8

```console
$ docker pull elixir@sha256:c9ae38510ce24ce9cf26795ac23879a2150bf106696ccfc5763805c0a8a0a160
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.9 MB (112856698 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:629a7f260deebac579572bc68a6f671a6c0bdd0fdbceb7ffb6ad134defe8ea03`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 22 Jul 2020 00:40:37 GMT
ADD file:14b8dca0bc0e6dae2f0bdb018a3a4e6d8d041abd03d118ae27cf7a72668f4970 in / 
# Wed, 22 Jul 2020 00:40:41 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 02:06:52 GMT
ENV OTP_VERSION=22.3.4.3
# Wed, 22 Jul 2020 02:06:53 GMT
LABEL org.opencontainers.image.version=22.3.4.3
# Wed, 22 Jul 2020 02:13:39 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="557376f7fef07fd7f08eedebcd23de8c921d7dfc9430e214d29a4726d92537d2" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 22 Jul 2020 02:13:42 GMT
CMD ["erl"]
# Thu, 23 Jul 2020 00:14:05 GMT
ENV ELIXIR_VERSION=v1.10.4 LANG=C.UTF-8
# Thu, 23 Jul 2020 00:16:53 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="8518c78f43fe36315dbe0d623823c2c1b7a025c114f3f4adbb48e04ef63f1d9f" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Jul 2020 00:16:56 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:e2b2cb832ad58353bcc4edbdd16023beb64ec7856b469d202975f8de836c6906`  
		Last Modified: Wed, 22 Jul 2020 00:47:20 GMT  
		Size: 49.2 MB (49168473 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:742003b5c3d93761aa88079de3b10da6cdc0c46be802d6eb5fa6499e2e700d5c`  
		Last Modified: Wed, 22 Jul 2020 03:49:09 GMT  
		Size: 56.4 MB (56445527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7dd8408061a4052e4e7892b22c5fbb71e4d724d511326c712bbcf2bf81587d36`  
		Last Modified: Thu, 23 Jul 2020 00:40:44 GMT  
		Size: 7.2 MB (7242698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; 386

```console
$ docker pull elixir@sha256:fc1d9309e2b834bb0fa7c43bf1a8820459603d982cede1cba1e5b5dba9d0a3e8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.3 MB (117277403 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:95e6d4767418c7f14191e719be356e6d89abfce7bba2564a87da76b5061542f0`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 22 Jul 2020 02:08:55 GMT
ADD file:2f4b8d9ab41b6e158f5926883b6bffdab1757086d903f3f0244f75bafc2e4876 in / 
# Wed, 22 Jul 2020 02:08:56 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 04:46:01 GMT
ENV OTP_VERSION=22.3.4.3
# Wed, 22 Jul 2020 04:46:01 GMT
LABEL org.opencontainers.image.version=22.3.4.3
# Wed, 22 Jul 2020 05:07:23 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="557376f7fef07fd7f08eedebcd23de8c921d7dfc9430e214d29a4726d92537d2" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 22 Jul 2020 05:07:24 GMT
CMD ["erl"]
# Wed, 22 Jul 2020 21:56:46 GMT
ENV ELIXIR_VERSION=v1.10.4 LANG=C.UTF-8
# Wed, 22 Jul 2020 21:58:25 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="8518c78f43fe36315dbe0d623823c2c1b7a025c114f3f4adbb48e04ef63f1d9f" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 21:58:25 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:88151d2519867746e4945a0a06b45430b9ddc2ae4be7e7f927cc00e3f640290d`  
		Last Modified: Wed, 22 Jul 2020 02:15:24 GMT  
		Size: 51.2 MB (51157197 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aebf68f1d532c9fb45a6b45c9986964f26ab57d2291011a8fc49c39e9dcafab9`  
		Last Modified: Wed, 22 Jul 2020 07:52:01 GMT  
		Size: 58.9 MB (58877649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84f1aca1d79010abda7e3c545940751ae1eb188ef8f38e6c895332d72a4d1313`  
		Last Modified: Wed, 22 Jul 2020 22:15:25 GMT  
		Size: 7.2 MB (7242557 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; ppc64le

```console
$ docker pull elixir@sha256:ecf17cffe011720c82ef0195f16c21ba5d6f0800fe2e9814a1c8fd38901b8265
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118739931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0e3c55520bb10a615c84f1abc6004e851027795aeee6414ad5628b565df7bc35`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 22 Jul 2020 02:15:14 GMT
ADD file:3e8bf6319c2535d9da6756a6f316eac0a488312c1297fdd54c9e064959e50da8 in / 
# Wed, 22 Jul 2020 02:15:27 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 04:33:55 GMT
ENV OTP_VERSION=22.3.4.3
# Wed, 22 Jul 2020 04:33:59 GMT
LABEL org.opencontainers.image.version=22.3.4.3
# Wed, 22 Jul 2020 04:47:12 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="557376f7fef07fd7f08eedebcd23de8c921d7dfc9430e214d29a4726d92537d2" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 22 Jul 2020 04:47:21 GMT
CMD ["erl"]
# Wed, 22 Jul 2020 18:06:18 GMT
ENV ELIXIR_VERSION=v1.10.4 LANG=C.UTF-8
# Wed, 22 Jul 2020 18:09:49 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="8518c78f43fe36315dbe0d623823c2c1b7a025c114f3f4adbb48e04ef63f1d9f" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 18:09:52 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:1c8685784756ef2cf52bfd7aa4cf826bd407c500b8402bd2b5b799a2e734e133`  
		Last Modified: Wed, 22 Jul 2020 02:24:38 GMT  
		Size: 54.1 MB (54143905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b997dbba953fe5250d88155505117e71998adec350a62fb9b5539d6a5d7597a`  
		Last Modified: Wed, 22 Jul 2020 04:49:19 GMT  
		Size: 57.4 MB (57352412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2db429652722922872b75bcb4f9671ba7e51393dabe38e4b6944582e8afcf1f7`  
		Last Modified: Wed, 22 Jul 2020 18:17:20 GMT  
		Size: 7.2 MB (7243614 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; s390x

```console
$ docker pull elixir@sha256:26b0fba5831fb3e2e13e85552a9da7144b3c0395ca0d435646c9433125fe23b3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.7 MB (112697896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ad4f6f214b8dea421a4bea0192e591f23107a6de3d3c851d6a67d5d9bbb973b`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 22 Jul 2020 00:42:24 GMT
ADD file:e5fcdcbbd996899922beac57e202b7e0895321e07263147e96c6e3b7b811d8a2 in / 
# Wed, 22 Jul 2020 00:42:26 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 04:40:55 GMT
ENV OTP_VERSION=22.3.4.3
# Wed, 22 Jul 2020 04:40:55 GMT
LABEL org.opencontainers.image.version=22.3.4.3
# Wed, 22 Jul 2020 04:45:07 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="557376f7fef07fd7f08eedebcd23de8c921d7dfc9430e214d29a4726d92537d2" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 22 Jul 2020 04:45:09 GMT
CMD ["erl"]
# Wed, 22 Jul 2020 10:25:47 GMT
ENV ELIXIR_VERSION=v1.10.4 LANG=C.UTF-8
# Wed, 22 Jul 2020 10:27:03 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="8518c78f43fe36315dbe0d623823c2c1b7a025c114f3f4adbb48e04ef63f1d9f" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 10:27:04 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:7ecdd8436fd4d951f4ca002a2aa8b01d427a7c4b535083e3ef0792444053154d`  
		Last Modified: Wed, 22 Jul 2020 00:45:30 GMT  
		Size: 49.0 MB (48966422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3f67e6e5044d4869d9f47f25c032848759338078f23897045d2dd532cb7e94`  
		Last Modified: Wed, 22 Jul 2020 04:48:03 GMT  
		Size: 56.5 MB (56489122 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df069f865be0af681f852de0d0785134a137e130d00fcd3f1d9b483c22b47b1b`  
		Last Modified: Wed, 22 Jul 2020 10:32:40 GMT  
		Size: 7.2 MB (7242352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
