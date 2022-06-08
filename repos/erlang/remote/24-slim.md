## `erlang:24-slim`

```console
$ docker pull erlang@sha256:be543ca05f729e2693390eede3d53f29732feebeebeb064c64c94e2b0f264602
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
$ docker pull erlang@sha256:2d92404b8bdd423a5be78b28259325ccf4c6f7e136d983f47645c418fd5b62ee
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.2 MB (120236886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:98049b754a056ae714272ceba33c7dd3886335ff792c658e864196811d855b46`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 May 2022 01:20:12 GMT
ADD file:dd3d4b31d7f1d4062ad0eb2d85dba064cea067b1eb4a8b89a0b593ea90001cdf in / 
# Sat, 28 May 2022 01:20:12 GMT
CMD ["bash"]
# Wed, 08 Jun 2022 21:27:24 GMT
ENV OTP_VERSION=24.3.4.1 REBAR3_VERSION=3.18.0
# Wed, 08 Jun 2022 21:27:24 GMT
LABEL org.opencontainers.image.version=24.3.4.1
# Wed, 08 Jun 2022 21:31:56 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="98363e5489356ed4fb3616e44d430b3daf5bb286be800d1c331fba8ef35ca3a0" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 08 Jun 2022 21:31:56 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:e756f3fdd6a378aa16205b0f75d178b7532b110e86be7659004fc6a21183226c`  
		Last Modified: Sat, 28 May 2022 01:24:51 GMT  
		Size: 55.0 MB (55009253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84063e10f58b847a0a0d0c577a1e07e90bcee55e2db46b719a0ad2ddbdbeb213`  
		Last Modified: Wed, 08 Jun 2022 21:39:54 GMT  
		Size: 65.2 MB (65227633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:24-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:b75909f1f96b7a10f283101dea1fde4cc730c753d7253a2c56291aef1785d2ca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.4 MB (107390533 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:40988c4ef84a28893e51f902c2038bb03bc373aaeae6621ef084f55b608114ca`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 May 2022 00:59:10 GMT
ADD file:faa82773e36b14c218e792730b0264c016864613a8d43cfaa33864075b0ef169 in / 
# Sat, 28 May 2022 00:59:11 GMT
CMD ["bash"]
# Wed, 08 Jun 2022 21:11:39 GMT
ENV OTP_VERSION=24.3.4.1 REBAR3_VERSION=3.18.0
# Wed, 08 Jun 2022 21:11:40 GMT
LABEL org.opencontainers.image.version=24.3.4.1
# Wed, 08 Jun 2022 21:19:58 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="98363e5489356ed4fb3616e44d430b3daf5bb286be800d1c331fba8ef35ca3a0" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 08 Jun 2022 21:19:58 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:8c8b1770c0de8d780b721bb37e9a8b6e5071a83530a584b1aed8ddc9aa12dd00`  
		Last Modified: Sat, 28 May 2022 01:14:50 GMT  
		Size: 50.2 MB (50199379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:077aeb2f9820d0a46fcc924ae9432e77138383d6206baffa8dce3d5a0bd7b186`  
		Last Modified: Wed, 08 Jun 2022 21:40:00 GMT  
		Size: 57.2 MB (57191154 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:24-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:2493502c7df55917c18a2706156eadad988470389e2dc4eca3220cdd5228915c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.8 MB (111752534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f23219cd02194f7eddbb4b310f534cac130abace46f2b690e100a24ce9d961e`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 May 2022 00:40:23 GMT
ADD file:a78273677555ebe8bac187f491203093eec62fa1c4f65f00ba2cf0cc2230992f in / 
# Sat, 28 May 2022 00:40:24 GMT
CMD ["bash"]
# Wed, 08 Jun 2022 20:46:17 GMT
ENV OTP_VERSION=24.3.4.1 REBAR3_VERSION=3.18.0
# Wed, 08 Jun 2022 20:46:18 GMT
LABEL org.opencontainers.image.version=24.3.4.1
# Wed, 08 Jun 2022 20:50:05 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="98363e5489356ed4fb3616e44d430b3daf5bb286be800d1c331fba8ef35ca3a0" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 08 Jun 2022 20:50:05 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:d794814721d57f8aaec06ab3652e90212cc3beccf5ff5c87f6ecf8375784bcc8`  
		Last Modified: Sat, 28 May 2022 00:47:04 GMT  
		Size: 53.7 MB (53696947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9872788e0a27fdd29ff0ba8876a1a171801754b5a0fdf6389190a589ec6a4888`  
		Last Modified: Wed, 08 Jun 2022 20:59:17 GMT  
		Size: 58.1 MB (58055587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:24-slim` - linux; 386

```console
$ docker pull erlang@sha256:e7b09947e388ca78a4ab77d7f677c0f38deb43cc35543302e4964f2176b3cf76
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.7 MB (113683382 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc7c4ae8ecd6f24f2fd776bcfd07e60a5dbd2ea5a75ff647091ed77dfb302ccc`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 May 2022 00:39:16 GMT
ADD file:2ecdc28ede565866b7302862c5e2a4b70a3afb165b383a4df315957be6dd754c in / 
# Sat, 28 May 2022 00:39:17 GMT
CMD ["bash"]
# Wed, 08 Jun 2022 20:47:06 GMT
ENV OTP_VERSION=24.3.4.1 REBAR3_VERSION=3.18.0
# Wed, 08 Jun 2022 20:47:07 GMT
LABEL org.opencontainers.image.version=24.3.4.1
# Wed, 08 Jun 2022 20:51:48 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="98363e5489356ed4fb3616e44d430b3daf5bb286be800d1c331fba8ef35ca3a0" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 08 Jun 2022 20:51:49 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:9460ac70d7d688bab5f76bf5c30d1d8577c1fe0b74778427b0febf82ec246360`  
		Last Modified: Sat, 28 May 2022 00:46:11 GMT  
		Size: 56.0 MB (56008088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:734451634f1cc2913505b972772f5da4fa3926bceb67bef5667e6c24fb939bcc`  
		Last Modified: Wed, 08 Jun 2022 21:02:18 GMT  
		Size: 57.7 MB (57675294 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:24-slim` - linux; ppc64le

```console
$ docker pull erlang@sha256:bb4da928c9d6bd23ff901012eae4d47b6563a3d088015a3e2dc2892370d9fa80
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.6 MB (117550246 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:891ff410585cf3f2231789dddf4a931e8c3afcacb8f633361ba45f71cf686172`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 May 2022 01:22:18 GMT
ADD file:0cf54bc63a3f2c0d5652c62456619ccdd983f64f718a89816c151963f108461f in / 
# Sat, 28 May 2022 01:22:26 GMT
CMD ["bash"]
# Wed, 08 Jun 2022 21:44:01 GMT
ENV OTP_VERSION=24.3.4.1 REBAR3_VERSION=3.18.0
# Wed, 08 Jun 2022 21:44:03 GMT
LABEL org.opencontainers.image.version=24.3.4.1
# Wed, 08 Jun 2022 21:53:02 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="98363e5489356ed4fb3616e44d430b3daf5bb286be800d1c331fba8ef35ca3a0" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 08 Jun 2022 21:53:07 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:6a8d10cab014c8bb87d1db1758eacc9d3a16b40994eec1e70e2eef174276708c`  
		Last Modified: Sat, 28 May 2022 01:31:45 GMT  
		Size: 58.9 MB (58902658 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:191087a8ee1cf565767964581a7cb348b8806689c149095cbb4017e0c95094a0`  
		Last Modified: Wed, 08 Jun 2022 22:04:38 GMT  
		Size: 58.6 MB (58647588 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:24-slim` - linux; s390x

```console
$ docker pull erlang@sha256:f998ec6f27758a98fec67dcedebf30ac45bbc31ba21b60fa9c73d8a9e4b1e8dc
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111443469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2790ed7a34f7bbaa3858d6e93df601bc2989cd383b8555bc7dc85326b0c0c66f`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 May 2022 00:42:39 GMT
ADD file:2aa6033cc58847736587260ccd8559fcc352cb0c91436fe6bc98ff1c0e457cc2 in / 
# Sat, 28 May 2022 00:42:42 GMT
CMD ["bash"]
# Wed, 08 Jun 2022 20:55:41 GMT
ENV OTP_VERSION=24.3.4.1 REBAR3_VERSION=3.18.0
# Wed, 08 Jun 2022 20:55:41 GMT
LABEL org.opencontainers.image.version=24.3.4.1
# Wed, 08 Jun 2022 21:02:37 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="98363e5489356ed4fb3616e44d430b3daf5bb286be800d1c331fba8ef35ca3a0" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 08 Jun 2022 21:02:42 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:5729889737c79e488091d7133428cefb547531cac87f70671a7a8def5c83b822`  
		Last Modified: Sat, 28 May 2022 00:49:25 GMT  
		Size: 53.3 MB (53276622 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3cc2885fd8c21658a2742febb11d90baf68e9dd07bff7dc469b9120feb508a3`  
		Last Modified: Wed, 08 Jun 2022 21:14:43 GMT  
		Size: 58.2 MB (58166847 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
