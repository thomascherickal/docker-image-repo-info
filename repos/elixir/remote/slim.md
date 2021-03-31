## `elixir:slim`

```console
$ docker pull elixir@sha256:9e4b8e77edc24e6761b758b29cbd6184146d64935c0cae30b1234ee071812966
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
$ docker pull elixir@sha256:0697490bbe7aa147a87c6c18b903d5f86e36894a357800d68d1fa9b65e1f2913
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118813713 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:18c11a0f1abd84c47ae7e20484bd26a5161e17b77404cb60706f94473e71ae35`
-	Default Command: `["iex"]`

```dockerfile
# Fri, 26 Mar 2021 15:20:41 GMT
ADD file:89234bb2f86c7eb890235a48904d1c9898a8d287a525c4fe5698d4a04cdd8f12 in / 
# Fri, 26 Mar 2021 15:20:42 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 18:47:58 GMT
ENV OTP_VERSION=23.3.1
# Tue, 30 Mar 2021 18:47:58 GMT
LABEL org.opencontainers.image.version=23.3.1
# Tue, 30 Mar 2021 19:03:18 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="a5a067a3b17bbef8511f2c056957925b666670b6f2cdaf645e1bc28ce3dd3517" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 30 Mar 2021 19:03:19 GMT
CMD ["erl"]
# Tue, 30 Mar 2021 21:04:53 GMT
ENV ELIXIR_VERSION=v1.11.4 LANG=C.UTF-8
# Tue, 30 Mar 2021 21:06:26 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="85c7118a0db6007507313db5bddf370216d9394ed7911fe80f21e2fbf7f54d29" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 21:06:26 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:8bf9c589d5f9475f1fcc050e02308d6b4eeb86eab7752ef948a13693e81a6aaa`  
		Last Modified: Fri, 26 Mar 2021 15:27:11 GMT  
		Size: 50.4 MB (50400278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71eff9c2f55f191ab83e502025cfffc8062f129e56b13e898e330f7fe05db15b`  
		Last Modified: Tue, 30 Mar 2021 20:07:44 GMT  
		Size: 60.9 MB (60922561 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4077c289eb28afca29c1393c910082e6306784ff20027c4c2ad7fb5d079852e`  
		Last Modified: Tue, 30 Mar 2021 21:17:21 GMT  
		Size: 7.5 MB (7490874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; arm variant v7

```console
$ docker pull elixir@sha256:1903168b363bd48432508a5ba91ee0760e5047b94928eb4c6561e18fdece7aca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.8 MB (112760611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3cfeeca5d8427610474952b0bca9e5b1db045643d1b40d57475a9f56c5f5a35e`
-	Default Command: `["iex"]`

```dockerfile
# Fri, 26 Mar 2021 11:17:10 GMT
ADD file:b3e1f7b8ae0587f7850210420c8dd6da7fb60fa87c5863e6fe5a8bab1bdc7abc in / 
# Fri, 26 Mar 2021 11:17:11 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 18:15:54 GMT
ENV OTP_VERSION=23.3.1
# Tue, 30 Mar 2021 18:15:55 GMT
LABEL org.opencontainers.image.version=23.3.1
# Tue, 30 Mar 2021 18:23:11 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="a5a067a3b17bbef8511f2c056957925b666670b6f2cdaf645e1bc28ce3dd3517" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 30 Mar 2021 18:23:15 GMT
CMD ["erl"]
# Tue, 30 Mar 2021 21:24:20 GMT
ENV ELIXIR_VERSION=v1.11.4 LANG=C.UTF-8
# Tue, 30 Mar 2021 21:26:58 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="85c7118a0db6007507313db5bddf370216d9394ed7911fe80f21e2fbf7f54d29" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 21:26:59 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:2703ee001e01b49055599d26cac8b1a472b75d8643e8a00ab281b97e3fe6aefd`  
		Last Modified: Fri, 26 Mar 2021 11:26:53 GMT  
		Size: 45.9 MB (45868006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4223863b3e2b216bb866c56ede035f95f7afd65a653db3c846f265a5a095faf`  
		Last Modified: Tue, 30 Mar 2021 19:04:19 GMT  
		Size: 59.4 MB (59402219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6ffec044ee04214dd906ef5c892b52f25867bb142ade820089cfb219062d23a`  
		Last Modified: Tue, 30 Mar 2021 21:43:24 GMT  
		Size: 7.5 MB (7490386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; arm64 variant v8

```console
$ docker pull elixir@sha256:05f346a4a2067f16df85f0d3797c435fa58a08d7f18a27c9d1c23a846d3a47a0
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.5 MB (114507457 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb3fcf616505557849e7e2d12eb53a3adc60a4c2970194aca3154e0acf1893b2`
-	Default Command: `["iex"]`

```dockerfile
# Fri, 26 Mar 2021 15:41:27 GMT
ADD file:536306ac674764a6a921b71adcbb4440797b916a0583b9270cd1565d62642e4d in / 
# Fri, 26 Mar 2021 15:41:30 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 17:55:00 GMT
ENV OTP_VERSION=23.3.1
# Tue, 30 Mar 2021 17:55:01 GMT
LABEL org.opencontainers.image.version=23.3.1
# Tue, 30 Mar 2021 18:01:22 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="a5a067a3b17bbef8511f2c056957925b666670b6f2cdaf645e1bc28ce3dd3517" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 30 Mar 2021 18:01:26 GMT
CMD ["erl"]
# Tue, 30 Mar 2021 20:21:25 GMT
ENV ELIXIR_VERSION=v1.11.4 LANG=C.UTF-8
# Tue, 30 Mar 2021 20:24:18 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="85c7118a0db6007507313db5bddf370216d9394ed7911fe80f21e2fbf7f54d29" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 20:24:20 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:383261dafcc4f63ecae5f2d661d1ef8d0a5e1c9f4b1f12285115baca7d101d5a`  
		Last Modified: Fri, 26 Mar 2021 15:48:21 GMT  
		Size: 49.2 MB (49196215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7896203b703adef7728a3b32884a34fac477d85818fa946d44e782b86a8e646b`  
		Last Modified: Tue, 30 Mar 2021 18:41:06 GMT  
		Size: 57.8 MB (57820556 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37c8b5d47e4dab13a266d97e636002d4a3d5d441105ca468103f4d3508420693`  
		Last Modified: Tue, 30 Mar 2021 20:41:36 GMT  
		Size: 7.5 MB (7490686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; 386

```console
$ docker pull elixir@sha256:539e6271bc06673b53f9b28e75dee940fc821bd8d84a04a81728a5f4a3f65f73
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.9 MB (118929833 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2864411c27f9f414813440a6d6dc3b082024eddb478033529e3ea0239e6a59b1`
-	Default Command: `["iex"]`

```dockerfile
# Fri, 26 Mar 2021 13:52:53 GMT
ADD file:631a0d940844da5859827f6532f16d070023eb5af86b98b26e8225892a728141 in / 
# Fri, 26 Mar 2021 13:52:53 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 17:55:34 GMT
ENV OTP_VERSION=23.3.1
# Tue, 30 Mar 2021 17:55:34 GMT
LABEL org.opencontainers.image.version=23.3.1
# Tue, 30 Mar 2021 18:03:34 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="a5a067a3b17bbef8511f2c056957925b666670b6f2cdaf645e1bc28ce3dd3517" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 30 Mar 2021 18:03:34 GMT
CMD ["erl"]
# Tue, 30 Mar 2021 20:22:23 GMT
ENV ELIXIR_VERSION=v1.11.4 LANG=C.UTF-8
# Tue, 30 Mar 2021 20:24:02 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="85c7118a0db6007507313db5bddf370216d9394ed7911fe80f21e2fbf7f54d29" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 20:24:02 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:94f8ae80c7bd585581d232dff8e781c1feaab54ea8d41718d95f0c1059908488`  
		Last Modified: Fri, 26 Mar 2021 14:00:56 GMT  
		Size: 51.2 MB (51160351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86b500700469b3215d152e7c4807d74ad469fe2d110aec2c8afed1f2f650e4a9`  
		Last Modified: Tue, 30 Mar 2021 19:17:09 GMT  
		Size: 60.3 MB (60278909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:577271a4a6dc8f4e8d98c01ba132dd3fd12225d27c54cc3311ebea81d094611c`  
		Last Modified: Tue, 30 Mar 2021 20:37:26 GMT  
		Size: 7.5 MB (7490573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; ppc64le

```console
$ docker pull elixir@sha256:bac1dc61ec8a98ec3e3a2d2af58a5cd492469aa087f9f2bed4f298cda3f49521
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **120.4 MB (120360755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37a2f47d730987975eff221bcfcd3463b8e0ad29ef7e5dd52baec987992fb485`
-	Default Command: `["iex"]`

```dockerfile
# Fri, 26 Mar 2021 15:13:48 GMT
ADD file:2e3cbe75ac7fb7b716e5b7411062bb9ce510f3317d00ddbfd608a5057931cc9a in / 
# Fri, 26 Mar 2021 15:13:55 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 18:41:02 GMT
ENV OTP_VERSION=23.3.1
# Tue, 30 Mar 2021 18:41:13 GMT
LABEL org.opencontainers.image.version=23.3.1
# Tue, 30 Mar 2021 18:57:30 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="a5a067a3b17bbef8511f2c056957925b666670b6f2cdaf645e1bc28ce3dd3517" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 30 Mar 2021 18:57:42 GMT
CMD ["erl"]
# Tue, 30 Mar 2021 22:15:50 GMT
ENV ELIXIR_VERSION=v1.11.4 LANG=C.UTF-8
# Tue, 30 Mar 2021 22:21:12 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="85c7118a0db6007507313db5bddf370216d9394ed7911fe80f21e2fbf7f54d29" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 22:21:17 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:2280757cb36e3eef6465890eb70453bb9f66e271e373f08ae5e9d7a3307c5fe4`  
		Last Modified: Fri, 26 Mar 2021 15:21:30 GMT  
		Size: 54.1 MB (54136619 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:032809e7ec644410340ae993a7fb3fbe0e731cf0af3b1220b274ff325af32f58`  
		Last Modified: Tue, 30 Mar 2021 19:09:02 GMT  
		Size: 58.7 MB (58732146 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f1285843e05724717fd07da05816f63ea3ce00fcea05b97c221ba02dbcbf4a3`  
		Last Modified: Tue, 30 Mar 2021 22:26:06 GMT  
		Size: 7.5 MB (7491990 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; s390x

```console
$ docker pull elixir@sha256:49f593cf4056175e9375b612e03afc9af1b07f2b34c3a38d1faa68c38997e746
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.3 MB (114330473 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4787dd08e1edd40db811ddaf0be0a9d3db7142eb86c87726732105f34a60288`
-	Default Command: `["iex"]`

```dockerfile
# Fri, 26 Mar 2021 10:53:31 GMT
ADD file:a8707fa1aa1620bd4a2cfb08af992575ed92583d76d9bc5cdf7512c966ef97ec in / 
# Fri, 26 Mar 2021 10:53:35 GMT
CMD ["bash"]
# Tue, 30 Mar 2021 17:53:32 GMT
ENV OTP_VERSION=23.3.1
# Tue, 30 Mar 2021 17:53:32 GMT
LABEL org.opencontainers.image.version=23.3.1
# Tue, 30 Mar 2021 17:58:55 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="a5a067a3b17bbef8511f2c056957925b666670b6f2cdaf645e1bc28ce3dd3517" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 30 Mar 2021 17:58:58 GMT
CMD ["erl"]
# Tue, 30 Mar 2021 19:40:40 GMT
ENV ELIXIR_VERSION=v1.11.4 LANG=C.UTF-8
# Tue, 30 Mar 2021 19:42:06 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="85c7118a0db6007507313db5bddf370216d9394ed7911fe80f21e2fbf7f54d29" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 30 Mar 2021 19:42:07 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:c1b0086a5cca01c7491d8c2f15dbad8cb1c1829a7d6d1edd7f8c3dd02be85f2b`  
		Last Modified: Fri, 26 Mar 2021 10:57:27 GMT  
		Size: 49.0 MB (48968913 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d51782e2f6bb790ec5b0ac86d9b6d0f5affa6b86aa60266a7468508263bb47e4`  
		Last Modified: Tue, 30 Mar 2021 18:07:07 GMT  
		Size: 57.9 MB (57871228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3550f0c0ad091b4daca9db955ad8c19f8ca4db62dfaca7d6bcf3a4f4b1174da`  
		Last Modified: Tue, 30 Mar 2021 19:44:47 GMT  
		Size: 7.5 MB (7490332 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
