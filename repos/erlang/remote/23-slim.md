## `erlang:23-slim`

```console
$ docker pull erlang@sha256:2c58819b70650fc3a565c0602e5724cfb9590f4216ad9ab33479d87d8905dcda
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
$ docker pull erlang@sha256:8c70edffbffcb3bdceb5bdc4d10ce077d07c657dd106772da4c8e38aaae2bb61
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.0 MB (111049528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03864cf5d5f4c873b897db1281f3ed79c5ff6c150183d49d48f57975bffcf60c`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:58 GMT
ADD file:9a4fd72d749f4a791e75e0f6fc6028d0771e3381b6d84a8d0b07a4887bc7c641 in / 
# Tue, 17 Nov 2020 20:20:58 GMT
CMD ["bash"]
# Wed, 09 Dec 2020 02:33:44 GMT
ENV OTP_VERSION=23.1.5
# Wed, 09 Dec 2020 02:33:44 GMT
LABEL org.opencontainers.image.version=23.1.5
# Wed, 09 Dec 2020 02:45:07 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="31719b8681e7f9ad6f30e329a0a0e5c4dd23dea858021573395fcdbea0d7702c" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 09 Dec 2020 02:45:07 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:756975cb9c7e7933d824af9319b512dd72a50894232761d06ef3be59981df838`  
		Last Modified: Tue, 17 Nov 2020 20:27:06 GMT  
		Size: 50.4 MB (50397725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f07d6edee27f3c924ad0040d3e9d041b758e26d74d2ebb3c3c911785d74e065`  
		Last Modified: Wed, 09 Dec 2020 04:05:37 GMT  
		Size: 60.7 MB (60651803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:f3880f10d0d13a011380ed0cd90cce6d047bf40ba58c15febf2404a47771b70c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.3 MB (102317288 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8f1b41dd1c2f503c2568370bcfb0a094e57c401f3da4ca6c91511f4ffce15699`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 17 Nov 2020 20:20:30 GMT
ADD file:81141d8fa450e1e5af67bb3757057f3fc34d3ed35cfd0caedb0aab64c5da9aaf in / 
# Tue, 17 Nov 2020 20:20:33 GMT
CMD ["bash"]
# Wed, 09 Dec 2020 02:10:40 GMT
ENV OTP_VERSION=23.1.5
# Wed, 09 Dec 2020 02:10:41 GMT
LABEL org.opencontainers.image.version=23.1.5
# Wed, 09 Dec 2020 02:17:16 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="31719b8681e7f9ad6f30e329a0a0e5c4dd23dea858021573395fcdbea0d7702c" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 09 Dec 2020 02:17:19 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:ebde10b2510128140d24e66909ceb0c80e00656af313829f82d31ae8cf08bcf8`  
		Last Modified: Tue, 17 Nov 2020 20:31:13 GMT  
		Size: 45.9 MB (45868212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f57d56a7e51e0f902b66fd5087beb2da76008e930692161325830a04e453a3c`  
		Last Modified: Wed, 09 Dec 2020 02:47:44 GMT  
		Size: 56.4 MB (56449076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:10e887ba81d59ece079c25e21ccecb6dda4923c47b7892c599c63155969a8d05
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106748786 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e260b07459ff4c4ba68fcb35b9197def0bfe3b98bf9d89389a0d6fd2a169cb3`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 17 Nov 2020 20:23:04 GMT
ADD file:28343d2066831f0ffb2002914f158698f92b4af6dc16ac22e3d8e9c388c688bb in / 
# Tue, 17 Nov 2020 20:23:05 GMT
CMD ["bash"]
# Wed, 09 Dec 2020 02:51:00 GMT
ENV OTP_VERSION=23.1.5
# Wed, 09 Dec 2020 02:51:00 GMT
LABEL org.opencontainers.image.version=23.1.5
# Wed, 09 Dec 2020 02:57:32 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="31719b8681e7f9ad6f30e329a0a0e5c4dd23dea858021573395fcdbea0d7702c" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 09 Dec 2020 02:57:34 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:22518ad4a7da48a5acd01946dad2fbee99e4fca910d23b78cd7e4a16c3bd1e5b`  
		Last Modified: Tue, 17 Nov 2020 20:31:35 GMT  
		Size: 49.2 MB (49179215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4276815afcf7d9059462dbc960b90b78c7e6a94f78132ad72606b901807a009`  
		Last Modified: Wed, 09 Dec 2020 03:26:41 GMT  
		Size: 57.6 MB (57569571 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; 386

```console
$ docker pull erlang@sha256:e22b1b0f65a95f5fcfdf2270cabaf7660c49b9e585675291695618281b539abe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.2 MB (111173061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cc936ce0cf9cdc4f3dfba15287816cb0fad955b45a186b5d2659ecdbefe38f7d`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 17 Nov 2020 20:19:39 GMT
ADD file:4805e11ec22df9454eb4759523111e031e84c8078bcaef178f089baca9e83cdb in / 
# Tue, 17 Nov 2020 20:19:40 GMT
CMD ["bash"]
# Wed, 09 Dec 2020 03:04:21 GMT
ENV OTP_VERSION=23.1.5
# Wed, 09 Dec 2020 03:04:22 GMT
LABEL org.opencontainers.image.version=23.1.5
# Wed, 09 Dec 2020 03:21:50 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="31719b8681e7f9ad6f30e329a0a0e5c4dd23dea858021573395fcdbea0d7702c" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 09 Dec 2020 03:21:50 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:21c39c42a8e082b1b164b44e463e4752c74821dbc51451f2ac2518ae6f29dff3`  
		Last Modified: Tue, 17 Nov 2020 20:26:25 GMT  
		Size: 51.2 MB (51159492 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56701f19d1cf833e0da376b2a7bc4e4c0eedf77ea75c67c831262ab1cf2fcba0`  
		Last Modified: Wed, 09 Dec 2020 04:37:30 GMT  
		Size: 60.0 MB (60013569 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; ppc64le

```console
$ docker pull erlang@sha256:558d97b6704fabc087d03bdd04bfa2fd08b1653296160951b57eb9bd243b92f2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.7 MB (112655692 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:68011d766f06cbd96500b6f424d76a91e82cf42a2ec864a12387b0daafc5b173`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 17 Nov 2020 23:22:28 GMT
ADD file:b5112ae3b22de1d8a373191ad01151a6c1cdde605887b1836672be39787e2213 in / 
# Tue, 17 Nov 2020 23:22:37 GMT
CMD ["bash"]
# Wed, 09 Dec 2020 03:03:14 GMT
ENV OTP_VERSION=23.1.5
# Wed, 09 Dec 2020 03:03:21 GMT
LABEL org.opencontainers.image.version=23.1.5
# Wed, 09 Dec 2020 03:35:20 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="31719b8681e7f9ad6f30e329a0a0e5c4dd23dea858021573395fcdbea0d7702c" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 09 Dec 2020 03:35:40 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:94e00adb98ff1f971add74025ff2a8ca87e003568d828bdb0df26ecd46c269a2`  
		Last Modified: Tue, 17 Nov 2020 23:31:43 GMT  
		Size: 54.1 MB (54143125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4d10af056a55a6cee29dfd3e8d36d1d19b27927baeee0fbdce87a34a68b0eac`  
		Last Modified: Wed, 09 Dec 2020 04:55:47 GMT  
		Size: 58.5 MB (58512567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-slim` - linux; s390x

```console
$ docker pull erlang@sha256:e0a4f8c8ae98214b4f170d7dd4d00749f236922b8a15ddd964304ad4f1786e4d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.6 MB (106567849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20530743022be71db5cda4b9e376a6e2c96f19e690d219422c90a48135b7a674`
-	Default Command: `["erl"]`

```dockerfile
# Fri, 11 Dec 2020 02:11:47 GMT
ADD file:b48379f9d2c111607924e8c59c2769c735341a59df0d6819d8a4b3e44f5457b0 in / 
# Fri, 11 Dec 2020 02:11:54 GMT
CMD ["bash"]
# Fri, 11 Dec 2020 02:45:40 GMT
ENV OTP_VERSION=23.1.5
# Fri, 11 Dec 2020 02:45:41 GMT
LABEL org.opencontainers.image.version=23.1.5
# Fri, 11 Dec 2020 02:53:05 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="31719b8681e7f9ad6f30e329a0a0e5c4dd23dea858021573395fcdbea0d7702c" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 11 Dec 2020 02:53:13 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:b8cd59e115fe85cdffdb9750beb150c189e768249dc100d22cab4733fb0c7247`  
		Last Modified: Fri, 11 Dec 2020 02:16:44 GMT  
		Size: 49.0 MB (48968242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b929cf226bed6ca69d130a044dffdd3f0cc7e0cbd5013603790baa93ad958ba`  
		Last Modified: Fri, 11 Dec 2020 03:09:43 GMT  
		Size: 57.6 MB (57599607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
