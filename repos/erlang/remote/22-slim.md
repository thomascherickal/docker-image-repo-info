## `erlang:22-slim`

```console
$ docker pull erlang@sha256:d35232ca0ed78d743f1529393f59ae723ff97f088804442e9a0cf9a219f3293e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `erlang:22-slim` - linux; amd64

```console
$ docker pull erlang@sha256:a32afebe762f30cc9ce131f851254bd3549a2e9e41716eeef0ce9addc90c5409
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109777216 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:48f5077e9a0ae2f9ab26ac8b6991e1f72bcd1d3aeb1387dc8d1bdc929c444751`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:08 GMT
ADD file:d6d0bdf8cb07a7a0dc32e9df50ac80ca1a524c3fa48136892ded195061f2194c in / 
# Sat, 28 Dec 2019 04:21:09 GMT
CMD ["bash"]
# Wed, 29 Jan 2020 01:32:30 GMT
ENV OTP_VERSION=22.2.4
# Wed, 29 Jan 2020 01:32:30 GMT
LABEL org.opencontainers.image.version=22.2.4
# Wed, 29 Jan 2020 01:48:08 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="7aab2285b46462332a7fdad395d4629e6465d5da324cf7e081e8d62fdb5b38f1" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 29 Jan 2020 01:48:08 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:8f0fdd3eaac017684c880d836abdaf02f9db7ac8ecca970356482e3d8e315650`  
		Last Modified: Sat, 28 Dec 2019 04:25:39 GMT  
		Size: 50.4 MB (50379720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63947aeb6e514353841ca0df1b9d2d8fc87b717e7b7bb4bb6a4635e730d27aaf`  
		Last Modified: Wed, 29 Jan 2020 02:10:10 GMT  
		Size: 59.4 MB (59397496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:22-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:bdf5b190397718934f4008cd7f60833cf75891578914f4ca87faacc1139732e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.0 MB (101010176 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ca7956d916cd5912a4f893e2daab8094c2d5adfc601ce8d4856e17fdbc5e011c`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:58:42 GMT
ADD file:26fba5cd6ba1fe45f19fb80d1c8e54eac5189e2b93e521b2ba6d5a6b54175e81 in / 
# Sat, 28 Dec 2019 04:58:45 GMT
CMD ["bash"]
# Wed, 29 Jan 2020 02:07:20 GMT
ENV OTP_VERSION=22.2.4
# Wed, 29 Jan 2020 02:07:21 GMT
LABEL org.opencontainers.image.version=22.2.4
# Wed, 29 Jan 2020 02:13:41 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="7aab2285b46462332a7fdad395d4629e6465d5da324cf7e081e8d62fdb5b38f1" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 29 Jan 2020 02:13:43 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:760e5af4a2ec2472d42b6773d075af9d2a006e0b7725ba9992e530f561d326f8`  
		Last Modified: Sat, 28 Dec 2019 05:07:11 GMT  
		Size: 45.9 MB (45859628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d812b5d2300255c745878f2ace159c872b47072f17a302d68d1f9509d3a1ea9f`  
		Last Modified: Wed, 29 Jan 2020 02:21:49 GMT  
		Size: 55.2 MB (55150548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:22-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:5b580784927dc812978deb7527cc5b71da052be8e15c51fd2242ac6d36681144
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.5 MB (105479667 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06e487e87be08eae5ae44050dea80e8b79ca299df72ce7cfaa990342073da6f5`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:40:41 GMT
ADD file:88b3d02fc98aa9138e694bee7d5d1b61b295e4a1c7fae399bf24e52eeff7a5ae in / 
# Sat, 28 Dec 2019 04:40:45 GMT
CMD ["bash"]
# Wed, 29 Jan 2020 01:48:42 GMT
ENV OTP_VERSION=22.2.4
# Wed, 29 Jan 2020 01:48:42 GMT
LABEL org.opencontainers.image.version=22.2.4
# Wed, 29 Jan 2020 01:54:47 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="7aab2285b46462332a7fdad395d4629e6465d5da324cf7e081e8d62fdb5b38f1" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 29 Jan 2020 01:54:49 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:627706d65d1d9b4038d8fd40db52238d4f11d9130a01f23ffae9bf5d41ac5933`  
		Last Modified: Sat, 28 Dec 2019 04:46:38 GMT  
		Size: 49.2 MB (49171876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be2d84de2bd7756a66ed84cadc579e5f07b1691e15461209bfbe659f55708057`  
		Last Modified: Wed, 29 Jan 2020 02:03:19 GMT  
		Size: 56.3 MB (56307791 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:22-slim` - linux; 386

```console
$ docker pull erlang@sha256:ad0b7f637edf75332658c760a27fa1948674541de9da73d616b57d8155bac69a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109896898 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1c7b5110804d26ed5c9975e93689fed984554c6a25bcc986c3b5812b5815a05`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:20 GMT
ADD file:c2d3c2cbbc436161afbcdcab7f07d11962ae8a6e99f8ed2c4ff2bcc92455a406 in / 
# Sat, 28 Dec 2019 04:39:21 GMT
CMD ["bash"]
# Wed, 29 Jan 2020 02:03:54 GMT
ENV OTP_VERSION=22.2.4
# Wed, 29 Jan 2020 02:03:54 GMT
LABEL org.opencontainers.image.version=22.2.4
# Wed, 29 Jan 2020 02:18:11 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="7aab2285b46462332a7fdad395d4629e6465d5da324cf7e081e8d62fdb5b38f1" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 29 Jan 2020 02:18:11 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:b3ff5188aae7f0986a4e7385f8249878f585ef70be99706b3262795514448afc`  
		Last Modified: Sat, 28 Dec 2019 04:44:08 GMT  
		Size: 51.1 MB (51141961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a2031fbcfc4b4918e16e0b56d7d1ec78d606c7d27d298685bc1a0fcb13926ba`  
		Last Modified: Wed, 29 Jan 2020 02:35:53 GMT  
		Size: 58.8 MB (58754937 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:22-slim` - linux; ppc64le

```console
$ docker pull erlang@sha256:3c3327d2495afeceeefc6d437c57e63d10e3e851ad8834b0bb7a0788e407fbe2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **111.3 MB (111335823 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1522b8149f9ee3134a542408aaeba4f2527e0ed0d88d5fdef8efc915584b8dd`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:12 GMT
ADD file:7c5858835ffb42e32df47084d7f85ba9392c5e37ee636e19dfae15d858c5b6c4 in / 
# Sat, 28 Dec 2019 04:20:17 GMT
CMD ["bash"]
# Wed, 22 Jan 2020 01:28:42 GMT
ENV OTP_VERSION=22.2.3
# Wed, 22 Jan 2020 01:28:44 GMT
LABEL org.opencontainers.image.version=22.2.3
# Wed, 22 Jan 2020 01:37:54 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="8470fff519d9ffa5defba4e42c3c1e64cd86905313040246d4a6e35799a9e614" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 22 Jan 2020 01:37:58 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:0a9adf09915c3544b1264f206aec99890c8e5e5c358fc4327886fbdab3c9eecc`  
		Last Modified: Sat, 28 Dec 2019 04:27:21 GMT  
		Size: 54.1 MB (54132515 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22b1de846f94094437ba3949e60a2b6b78c08687e5477a70d5298526804af8f2`  
		Last Modified: Wed, 22 Jan 2020 02:49:05 GMT  
		Size: 57.2 MB (57203308 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:22-slim` - linux; s390x

```console
$ docker pull erlang@sha256:8f97c39f9c4328e5ff632f51b99953975ad4b1e49e7ccb5c20654db4186fef74
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105277577 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e52f9de958939da4e878b947c2636a0a42edb60af3b40ae4b25055932050073e`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:51 GMT
ADD file:aeaf0b11195b2ba7eb7890ce128ad93c114a8e183a516cf2e4ea42da324c57ea in / 
# Sat, 28 Dec 2019 04:41:51 GMT
CMD ["bash"]
# Wed, 29 Jan 2020 01:48:45 GMT
ENV OTP_VERSION=22.2.4
# Wed, 29 Jan 2020 01:48:46 GMT
LABEL org.opencontainers.image.version=22.2.4
# Wed, 29 Jan 2020 01:52:36 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="7aab2285b46462332a7fdad395d4629e6465d5da324cf7e081e8d62fdb5b38f1" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 29 Jan 2020 01:52:38 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:3596c5a237f76c32832c1879a3d0c763989cb13fac0024673b03e9b549b868ea`  
		Last Modified: Sat, 28 Dec 2019 04:44:54 GMT  
		Size: 49.0 MB (48954508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc886e8c55eb1682d0bba8a86f214869836e3f7495a32ceedee4bf6de5fd388d`  
		Last Modified: Wed, 29 Jan 2020 01:59:07 GMT  
		Size: 56.3 MB (56323069 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
