## `erlang:25-slim`

```console
$ docker pull erlang@sha256:a0305fe80aa92f7c1afbe9f26b085618b4e5843a6c3158fb1f328eeced7fc137
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `erlang:25-slim` - linux; amd64

```console
$ docker pull erlang@sha256:1d59ba451779247aa06043efefd325000d80a2b502aa14345901d088506af98a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.6 MB (120573174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:63c161aec263f35e9ec5bcf34b651f10391172d41ff2a542c20b71ced1657c1e`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 02 Aug 2022 01:19:54 GMT
ADD file:d0f758e50c654c225f6c7f03e8a579efc9106437051573bdbae5e63b1c4b2c1f in / 
# Tue, 02 Aug 2022 01:19:54 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:38:48 GMT
ENV OTP_VERSION=25.0.3 REBAR3_VERSION=3.18.0
# Tue, 02 Aug 2022 02:38:48 GMT
LABEL org.opencontainers.image.version=25.0.3
# Tue, 02 Aug 2022 02:43:32 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e8eca69b6bdaac9cc8f3e3177dd2913920513495ee83bdecf73af546768febd6" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:43:33 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:001c52e26ad57e3b25b439ee0052f6692e5c0f2d5d982a00a8819ace5e521452`  
		Last Modified: Tue, 02 Aug 2022 01:23:44 GMT  
		Size: 55.0 MB (54999331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48127bafd2b2a971f4ee9f6388d7980d654ea17a814ec1e185a2aac9e7de1b3d`  
		Last Modified: Tue, 02 Aug 2022 04:00:17 GMT  
		Size: 65.6 MB (65573843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:25-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:d1bc37319cc7f002f86fc480f49bb66791c8572443fd12dda3e871dc7863fd11
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107103585 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c94affe040c10f0c88c1e789d6dac352649d22d99a1b9ba321797e10741a0d7`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 12 Jul 2022 00:59:16 GMT
ADD file:72ef8362158fcd45f10c6fa2dc3ea411e81f700ecb92faf37cb6dc1887756f9d in / 
# Tue, 12 Jul 2022 00:59:17 GMT
CMD ["bash"]
# Fri, 29 Jul 2022 03:21:14 GMT
ENV OTP_VERSION=25.0.3 REBAR3_VERSION=3.18.0
# Fri, 29 Jul 2022 03:21:14 GMT
LABEL org.opencontainers.image.version=25.0.3
# Fri, 29 Jul 2022 03:33:36 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e8eca69b6bdaac9cc8f3e3177dd2913920513495ee83bdecf73af546768febd6" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 29 Jul 2022 03:33:36 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:a8a55ed160b9a554de2e46b828d606a0829d8d9f19c79bc47eddac683aeb2b91`  
		Last Modified: Tue, 12 Jul 2022 01:11:51 GMT  
		Size: 50.2 MB (50194881 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebcd354acf6bbfb49bc727556dee5475aa8d0654e27b27b7f6f09cad8db117d7`  
		Last Modified: Fri, 29 Jul 2022 06:42:36 GMT  
		Size: 56.9 MB (56908704 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:25-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:cd322ab082cd3d6bcbdb5b2f3071104a776b3a40b9cd63040af382a96bd26395
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.7 MB (117685380 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f0428dbc279de4f29267a72d2e9aeaf607c6538d1467e08cc333550abb7675`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 02 Aug 2022 00:40:24 GMT
ADD file:5972a7ce0f1d89d63e5ed48011838c998fa506cd34f8e5f0b0070039cd74c5b9 in / 
# Tue, 02 Aug 2022 00:40:25 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 02:09:19 GMT
ENV OTP_VERSION=25.0.3 REBAR3_VERSION=3.18.0
# Tue, 02 Aug 2022 02:09:20 GMT
LABEL org.opencontainers.image.version=25.0.3
# Tue, 02 Aug 2022 02:13:24 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e8eca69b6bdaac9cc8f3e3177dd2913920513495ee83bdecf73af546768febd6" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 02 Aug 2022 02:13:25 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:114ba63dd73a866ac1bb59fe594dfd218f44ac9b4fa4b2c68499da5584fcfa9d`  
		Last Modified: Tue, 02 Aug 2022 00:45:33 GMT  
		Size: 53.7 MB (53683005 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61d6bd9c7d658604ee3b78f6140196345171555b98bfb561e330de9b32eccf80`  
		Last Modified: Tue, 02 Aug 2022 03:09:34 GMT  
		Size: 64.0 MB (64002375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:25-slim` - linux; 386

```console
$ docker pull erlang@sha256:c5236c4cec2fbe5fc7a440a5aa0447b18b8834a7b8fcd488656020c31e7470ff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **113.3 MB (113305077 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3fafed1ac25006a4b44c25bf4ca81ec861ed70cc7448d9c2e872e1a7229b798`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 02 Aug 2022 00:39:05 GMT
ADD file:ade7fe80dd06354b3eab9283f6c354047be2b94806dbe1dedee8d5a0f658f7be in / 
# Tue, 02 Aug 2022 00:39:05 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:37:38 GMT
ENV OTP_VERSION=25.0.3 REBAR3_VERSION=3.18.0
# Tue, 02 Aug 2022 01:37:38 GMT
LABEL org.opencontainers.image.version=25.0.3
# Tue, 02 Aug 2022 01:42:32 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e8eca69b6bdaac9cc8f3e3177dd2913920513495ee83bdecf73af546768febd6" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:42:32 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:84601b97875630e4b14ebdb276bc4c68f89eafe6d12dec64b54dbcaed7c0c802`  
		Last Modified: Tue, 02 Aug 2022 00:44:40 GMT  
		Size: 56.0 MB (56002231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b41e92669d079de183f62fcf1378823b039aca5427c6895280ff1a087bad8549`  
		Last Modified: Tue, 02 Aug 2022 02:45:40 GMT  
		Size: 57.3 MB (57302846 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:25-slim` - linux; ppc64le

```console
$ docker pull erlang@sha256:e56a131d06311679b1541cb04556a01c6e307f1e2f2797201a94d50571c073cf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.1 MB (117146927 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ec919406af72309725a494903890feb0b88390362612bbd11f680076e1d6be3b`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 02 Aug 2022 01:17:09 GMT
ADD file:1f74997bc1d99e4422725846bbc41271bfe62a55c74ceca37359472aa428233c in / 
# Tue, 02 Aug 2022 01:17:12 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:48:08 GMT
ENV OTP_VERSION=25.0.3 REBAR3_VERSION=3.18.0
# Tue, 02 Aug 2022 01:48:09 GMT
LABEL org.opencontainers.image.version=25.0.3
# Tue, 02 Aug 2022 01:55:09 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e8eca69b6bdaac9cc8f3e3177dd2913920513495ee83bdecf73af546768febd6" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:55:11 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:6e9f012d4ab4ee25199c288014d1f6269e3700e4e09eb5ae543813498561f2fe`  
		Last Modified: Tue, 02 Aug 2022 01:24:00 GMT  
		Size: 58.9 MB (58895967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:814817f4ee3efdca4c00ceb74566971734149071ce76fd7b48cd98d077e38f25`  
		Last Modified: Tue, 02 Aug 2022 02:20:45 GMT  
		Size: 58.3 MB (58250960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:25-slim` - linux; s390x

```console
$ docker pull erlang@sha256:1c28ab3ab7f80a015f63ee4f4cb453c76de63b66d9c258e8202c5428f449d43b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.1 MB (111097073 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:931f3e4f224dd5826c5c62f855a3eb0101f755b04db2f697d7765c70041780db`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 02 Aug 2022 00:42:09 GMT
ADD file:86774aefa6717c0535c25f8700d8730f44cc43c33371edeb7dbd33e29cb68d32 in / 
# Tue, 02 Aug 2022 00:42:12 GMT
CMD ["bash"]
# Tue, 02 Aug 2022 01:48:29 GMT
ENV OTP_VERSION=25.0.3 REBAR3_VERSION=3.18.0
# Tue, 02 Aug 2022 01:48:29 GMT
LABEL org.opencontainers.image.version=25.0.3
# Tue, 02 Aug 2022 01:52:37 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e8eca69b6bdaac9cc8f3e3177dd2913920513495ee83bdecf73af546768febd6" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 02 Aug 2022 01:52:40 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:718eef7927531d5ec3c355d6b6e5c4ab83c23778e693b087ac8a3b9adb4f63e0`  
		Last Modified: Tue, 02 Aug 2022 00:47:40 GMT  
		Size: 53.3 MB (53269308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c0b831af94e2ed0a12c3a022a030de19ea8383d307fd2bd777e41b6eb8a8f51`  
		Last Modified: Tue, 02 Aug 2022 02:26:54 GMT  
		Size: 57.8 MB (57827765 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
