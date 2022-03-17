## `erlang:24-slim`

```console
$ docker pull erlang@sha256:08ac132187e46d5d92f5f935da625f1e9ba80e0e38b68dcfb10041756e3f513b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `erlang:24-slim` - linux; amd64

```console
$ docker pull erlang@sha256:35d654c2e72a27f045edcf1b34ab9c26805e2d8701ae88443e35329b5e27c102
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.0 MB (122030926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2eeb71eaad10cfb12319780cde769bed6325293907116d9988426bcdf72b0cd7`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 01 Mar 2022 02:13:15 GMT
ADD file:9c4db2a9644ee3029a8e9cca58350efef660c3167e59b91f2bee9c303e592664 in / 
# Tue, 01 Mar 2022 02:13:15 GMT
CMD ["bash"]
# Wed, 16 Mar 2022 18:37:02 GMT
ENV OTP_VERSION=24.3.1 REBAR3_VERSION=3.18.0
# Wed, 16 Mar 2022 18:37:02 GMT
LABEL org.opencontainers.image.version=24.3.1
# Wed, 16 Mar 2022 18:46:07 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="fb6f7c878c538d56588542abe1f069a29fecdbbca9701596a2d17636a0889db9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 16 Mar 2022 18:46:08 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:e4d61adff2077d048c6372d73c41b0bd68f525ad41f5530af05098a876683055`  
		Last Modified: Tue, 01 Mar 2022 02:18:55 GMT  
		Size: 54.9 MB (54917063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003942ff3025b48fe43934e0a49022bd6e43eeed41b24c1e9b0f1d88701a434f`  
		Last Modified: Wed, 16 Mar 2022 18:58:40 GMT  
		Size: 67.1 MB (67113863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:24-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:2ae2cfdca9b16de6618df7ff46b833f9fb4df09419d2f4c04075d084a15e4eb9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.8 MB (108841048 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11664c1fa7af0b47102dfa9caf9e8364fb15dddfae500df79d2ce52bc288719c`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 01 Mar 2022 02:02:17 GMT
ADD file:b388eaef074fa7cc4e0f6f0b6a56e4be6c69489b63477ab4469ff5415074b0c7 in / 
# Tue, 01 Mar 2022 02:02:18 GMT
CMD ["bash"]
# Wed, 16 Mar 2022 18:15:06 GMT
ENV OTP_VERSION=24.3.1 REBAR3_VERSION=3.18.0
# Wed, 16 Mar 2022 18:15:06 GMT
LABEL org.opencontainers.image.version=24.3.1
# Wed, 16 Mar 2022 18:23:21 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="fb6f7c878c538d56588542abe1f069a29fecdbbca9701596a2d17636a0889db9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 16 Mar 2022 18:23:21 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:17a41fc762495ca54ac53f271889bdf4ac8bea7cedfa3b585e4e42ef106935f1`  
		Last Modified: Tue, 01 Mar 2022 02:18:24 GMT  
		Size: 50.1 MB (50117069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:13edf20c6e3cba4bcc8ce22a5cb0e54449c54ecc23429c3b2d6f02caed9d75dc`  
		Last Modified: Wed, 16 Mar 2022 18:43:28 GMT  
		Size: 58.7 MB (58723979 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:24-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:c638d56667180a9cfe9e3171ed211c30bae08412b851df6f8a661b3c1c408ee9
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.2 MB (113211833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:592e59c9df379b865801813e3e6e95578b2c9d37128a52d85ebc28bd0bb49730`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 01 Mar 2022 02:11:12 GMT
ADD file:9d66afa8fc90803d689e087b38b38a3bd58d0434b495ca4165ca520e73bccf55 in / 
# Tue, 01 Mar 2022 02:11:14 GMT
CMD ["bash"]
# Wed, 16 Mar 2022 17:58:39 GMT
ENV OTP_VERSION=24.3.1 REBAR3_VERSION=3.18.0
# Wed, 16 Mar 2022 17:58:40 GMT
LABEL org.opencontainers.image.version=24.3.1
# Wed, 16 Mar 2022 18:02:25 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="fb6f7c878c538d56588542abe1f069a29fecdbbca9701596a2d17636a0889db9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 16 Mar 2022 18:02:25 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:c7869242ae9abf6340558e18846f64a05eb06f2eaf66c6bfa2dc66ff2c997976`  
		Last Modified: Tue, 01 Mar 2022 02:17:52 GMT  
		Size: 53.6 MB (53608753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a7533af76e2cd4df95eef9acf0fd350005c7a4d4d50644783b5507b9db307b9`  
		Last Modified: Wed, 16 Mar 2022 18:11:42 GMT  
		Size: 59.6 MB (59603080 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:24-slim` - linux; 386

```console
$ docker pull erlang@sha256:5c57cd3ac31c5e1d06d652b5e7f7efbdaf50bfd533ea7df66b5cddb3f823adfc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **115.5 MB (115508354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4fb5faa6509f3f05eabdd047eeb7a009585cb1fd9101419f9c12dc37ace3e0b`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 01 Mar 2022 02:07:15 GMT
ADD file:4341f64e7f1accc7f9737a9896bf50c6ba8f51698e52c594d9421fe4f2374e2a in / 
# Tue, 01 Mar 2022 02:07:15 GMT
CMD ["bash"]
# Wed, 16 Mar 2022 17:58:12 GMT
ENV OTP_VERSION=24.3.1 REBAR3_VERSION=3.18.0
# Wed, 16 Mar 2022 17:58:12 GMT
LABEL org.opencontainers.image.version=24.3.1
# Wed, 16 Mar 2022 18:05:18 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="fb6f7c878c538d56588542abe1f069a29fecdbbca9701596a2d17636a0889db9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 16 Mar 2022 18:05:18 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:5cf8159e9217c5f37fe58b260cacc1d132c2e21ca58c769d29c6eb720993a304`  
		Last Modified: Tue, 01 Mar 2022 02:15:15 GMT  
		Size: 55.9 MB (55938747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b64f4cd073802a35a39b3c61b415e03ad2906c8ed8eba3a6eff259e07a93f5f`  
		Last Modified: Wed, 16 Mar 2022 18:18:57 GMT  
		Size: 59.6 MB (59569607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:24-slim` - linux; ppc64le

```console
$ docker pull erlang@sha256:d825c4758b85d8b80071f2fc4f57b01211b8d10b59b49a3e9f56dc9673b5fb34
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.5 MB (119453909 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0e91a52d27e59db0f255a1063343d230aa8b94070417a8b474bfebbde4ee5c5`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 01 Mar 2022 02:04:22 GMT
ADD file:00554eaeb433a7cc43c22f2544d800896f451a2e5a7895863c4651ed425b8c36 in / 
# Tue, 01 Mar 2022 02:04:29 GMT
CMD ["bash"]
# Wed, 16 Mar 2022 19:26:01 GMT
ENV OTP_VERSION=24.3.1 REBAR3_VERSION=3.18.0
# Wed, 16 Mar 2022 19:26:05 GMT
LABEL org.opencontainers.image.version=24.3.1
# Wed, 16 Mar 2022 19:39:13 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="fb6f7c878c538d56588542abe1f069a29fecdbbca9701596a2d17636a0889db9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 16 Mar 2022 19:39:22 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:9ff352265b4a055377b95db6dddea03717bbefbc7f30fbacf493764d617ae85e`  
		Last Modified: Tue, 01 Mar 2022 02:14:41 GMT  
		Size: 58.8 MB (58834115 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5ea97b3429840a6492571994ea7ccd78d85b2df36c26e629cf8cd4a6f6d663d2`  
		Last Modified: Wed, 16 Mar 2022 19:50:58 GMT  
		Size: 60.6 MB (60619794 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:24-slim` - linux; s390x

```console
$ docker pull erlang@sha256:38382bd4d0f6327a3d9233df7380b2463a9bfedf12f9857caa8c511e85fb3ae3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111362707 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6aa8ceb13ce5f244a949117d66c3885e2290495e0bd45d01e5269bd34fb6aea9`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 17 Mar 2022 03:06:38 GMT
ADD file:75b45e65d2ec2c6822b1ddc46ff159dd10ac56bf9dff8b0996ac589a1ede22ff in / 
# Thu, 17 Mar 2022 03:06:42 GMT
CMD ["bash"]
# Thu, 17 Mar 2022 07:39:03 GMT
ENV OTP_VERSION=24.3.1 REBAR3_VERSION=3.18.0
# Thu, 17 Mar 2022 07:39:03 GMT
LABEL org.opencontainers.image.version=24.3.1
# Thu, 17 Mar 2022 07:42:58 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="fb6f7c878c538d56588542abe1f069a29fecdbbca9701596a2d17636a0889db9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 17 Mar 2022 07:43:01 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:ae9f1a186a2633be1ad71c317c2f195b221cef89502f9edc510b3a2049723758`  
		Last Modified: Thu, 17 Mar 2022 03:12:26 GMT  
		Size: 53.2 MB (53217527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95cdaf048bfcc52dc5efba7da691b130c7aaf970f529019fc1fb064a94ef6253`  
		Last Modified: Thu, 17 Mar 2022 07:59:05 GMT  
		Size: 58.1 MB (58145180 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
