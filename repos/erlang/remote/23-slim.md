## `erlang:23-slim`

```console
$ docker pull erlang@sha256:384eb9df82d920374f2b2759f643265e76b726a6710815d7ad850e5c8d12cc7c
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
$ docker pull erlang@sha256:22edc712971e08c70adf32bbd2faf7a867f250909957372415c6f4e8a5093b2d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.4 MB (111354450 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a8d64b269d7961fd6e25d74eb9ff498b4f828d9f4cd3b96e4163fd570d3f897e`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 10 Apr 2021 01:20:08 GMT
ADD file:e18bc3e10e7c743f18bb8be65ec94a62c03764af7dbdb4957f9a600237730212 in / 
# Sat, 10 Apr 2021 01:20:09 GMT
CMD ["bash"]
# Thu, 06 May 2021 18:44:05 GMT
ENV OTP_VERSION=23.3.3
# Thu, 06 May 2021 18:44:05 GMT
LABEL org.opencontainers.image.version=23.3.3
# Thu, 06 May 2021 18:59:24 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="839d74e71a457295d95b8674f1848a5d7d9c4c274a041ef8026d035da88858ae" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 06 May 2021 18:59:25 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:bd8f6a7501ccbe80b95c82519ed6fd4f7236a41e0ae59ba4a8df76af24629efc`  
		Last Modified: Sat, 10 Apr 2021 01:24:48 GMT  
		Size: 50.4 MB (50432971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3dbeff03fa6906c2c3646e7cde030559b88af3b7022c180a62383d4dfa6e73f`  
		Last Modified: Thu, 06 May 2021 21:15:00 GMT  
		Size: 60.9 MB (60921479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:aced984247f11a6979203044d4712235d86b1ec438d2e25b5f0d7ee3d464dfd8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105330249 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d0ff6801afb965b000019b03567ccf1fc23e139adaa5c3b667c3063ef7ef24ec`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 10 Apr 2021 00:59:18 GMT
ADD file:bd2081229497eea2b33310cb1582b965581ca78b00b87cc8e42bdc8b9f350678 in / 
# Sat, 10 Apr 2021 00:59:20 GMT
CMD ["bash"]
# Thu, 06 May 2021 18:16:11 GMT
ENV OTP_VERSION=23.3.3
# Thu, 06 May 2021 18:16:12 GMT
LABEL org.opencontainers.image.version=23.3.3
# Thu, 06 May 2021 18:26:03 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="839d74e71a457295d95b8674f1848a5d7d9c4c274a041ef8026d035da88858ae" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 06 May 2021 18:26:09 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:de0ca59eb81518ffd92fbcd386251018f950dc16b1bd8ad2e642184db76be2a1`  
		Last Modified: Sat, 10 Apr 2021 01:07:26 GMT  
		Size: 45.9 MB (45915598 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f245742982cf8504dc98a6fda390ddf6fabe495097f2b0f298e881b556ff8e3`  
		Last Modified: Thu, 06 May 2021 19:33:23 GMT  
		Size: 59.4 MB (59414651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:00b5276192a545b4d69a61ba9da549e2395af5f1fe6199982506b9056652c92e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.1 MB (107061908 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a3a9e7c4758582de73cd4837ef4f914674327739b0764207ee2de51eeae752c`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 10 Apr 2021 00:40:59 GMT
ADD file:320ad0e2a3d6c676ddb8ce5646b5a94d18d82a8868955da3a9379a261dfe1ffe in / 
# Sat, 10 Apr 2021 00:41:01 GMT
CMD ["bash"]
# Thu, 06 May 2021 17:51:15 GMT
ENV OTP_VERSION=23.3.3
# Thu, 06 May 2021 17:51:16 GMT
LABEL org.opencontainers.image.version=23.3.3
# Thu, 06 May 2021 17:57:50 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="839d74e71a457295d95b8674f1848a5d7d9c4c274a041ef8026d035da88858ae" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 06 May 2021 17:57:53 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:01cf0f0da10ede0eec0fc1c5fbfdeb63a447dfcc0a3c4419c0a4c3f0a2826636`  
		Last Modified: Sat, 10 Apr 2021 00:47:28 GMT  
		Size: 49.2 MB (49225782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199d4c7aa8fd3b86fc5844ae88180cb98ec192b05a317142f7b2d7e820c1f189`  
		Last Modified: Thu, 06 May 2021 19:09:24 GMT  
		Size: 57.8 MB (57836126 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; 386

```console
$ docker pull erlang@sha256:1a6a61bb2e07b8a77d2b55c0ea0beb9d3ba80750bc8b77a7a38277b0927b481d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.5 MB (111492456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b6d463a73ceb9293e1ec8cc25eee411411d4e42251a21eb9535e85c8740fdac3`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 10 Apr 2021 00:39:26 GMT
ADD file:de914d3ff1619f3af1574fb9644ffde6f0590dfcfe402ffc9e7b2c0500481706 in / 
# Sat, 10 Apr 2021 00:39:26 GMT
CMD ["bash"]
# Thu, 06 May 2021 17:51:51 GMT
ENV OTP_VERSION=23.3.3
# Thu, 06 May 2021 17:51:52 GMT
LABEL org.opencontainers.image.version=23.3.3
# Thu, 06 May 2021 17:59:32 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="839d74e71a457295d95b8674f1848a5d7d9c4c274a041ef8026d035da88858ae" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 06 May 2021 17:59:32 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:848aed59cb94060ff383c5bac16a4d69d7babe251466ce3f80195bf8f7209702`  
		Last Modified: Sat, 10 Apr 2021 00:45:25 GMT  
		Size: 51.2 MB (51198915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc449152d688a3718d356561130e2256ea965e4d5fd8a2874aec9d73ae12a6e5`  
		Last Modified: Thu, 06 May 2021 20:23:42 GMT  
		Size: 60.3 MB (60293541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; ppc64le

```console
$ docker pull erlang@sha256:14c62b7756144ecb3606bbf52f5d253783d89f11ca52f2c8cc0b9e4f4fb1faca
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.9 MB (112920673 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5b38883c628e2e9e9f53324bd3cf730ca088e3359969b5c7f6c7c9f341de64ed`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 10 Apr 2021 01:26:11 GMT
ADD file:0671a70f02e705f591888f40e87a43122cd95a6ead3df61becbc4a7fb1c7ec43 in / 
# Sat, 10 Apr 2021 01:26:21 GMT
CMD ["bash"]
# Thu, 06 May 2021 18:51:29 GMT
ENV OTP_VERSION=23.3.3
# Thu, 06 May 2021 18:51:36 GMT
LABEL org.opencontainers.image.version=23.3.3
# Thu, 06 May 2021 19:06:00 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="839d74e71a457295d95b8674f1848a5d7d9c4c274a041ef8026d035da88858ae" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 06 May 2021 19:06:09 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:d018a28ea8249b332e6bce3cb93862d5b05dba493dbaf3531505ce3a3701001b`  
		Last Modified: Sat, 10 Apr 2021 01:33:24 GMT  
		Size: 54.2 MB (54179922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e56e893220a1856a5c75a8bda2a6b3cbc0de08bc0009e32a3b8dd4d36e7f8dc`  
		Last Modified: Thu, 06 May 2021 20:11:05 GMT  
		Size: 58.7 MB (58740751 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; s390x

```console
$ docker pull erlang@sha256:54be02c35f6f8443c705232311b4ce6092c95c16cf4fafd0dfca907dc464404c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.9 MB (106885298 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e25addef8cabbba04d3964eed7d962a0d2f93fa1dcf99f381cc0c3d41fd19a6c`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 10 Apr 2021 00:42:07 GMT
ADD file:4df1e9998bf12ac6b068948127db30e29fdc3196e27d72adf972c6c1cc6ce2a0 in / 
# Sat, 10 Apr 2021 00:42:10 GMT
CMD ["bash"]
# Thu, 06 May 2021 18:00:33 GMT
ENV OTP_VERSION=23.3.3
# Thu, 06 May 2021 18:00:34 GMT
LABEL org.opencontainers.image.version=23.3.3
# Thu, 06 May 2021 18:09:48 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="839d74e71a457295d95b8674f1848a5d7d9c4c274a041ef8026d035da88858ae" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 06 May 2021 18:09:57 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:03bd9fa68773b62afcbde0348c41cadd08d602d2731d955581cc322351e8be39`  
		Last Modified: Sat, 10 Apr 2021 00:45:31 GMT  
		Size: 49.0 MB (49000527 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:319b8ace93b547a76511f7088a5973158d85cbdf7031b268730c4286e047ae44`  
		Last Modified: Thu, 06 May 2021 18:45:42 GMT  
		Size: 57.9 MB (57884771 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
