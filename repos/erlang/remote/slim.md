## `erlang:slim`

```console
$ docker pull erlang@sha256:cb10cd7df6227917fc4d1d3543f195fd533a1f89b555844ab18d7e2c26f07e84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `erlang:slim` - linux; amd64

```console
$ docker pull erlang@sha256:21ca23c8a4d28d9c58067014c39e6d542e63e69490c2eb3c1d648ab95c072e78
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.8 MB (109752791 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:864aa9ede6bd9707a1924b5624ae6254852a782d25b2e0d695a6d75151811df5`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:08 GMT
ADD file:d6d0bdf8cb07a7a0dc32e9df50ac80ca1a524c3fa48136892ded195061f2194c in / 
# Sat, 28 Dec 2019 04:21:09 GMT
CMD ["bash"]
# Tue, 14 Jan 2020 00:32:48 GMT
ENV OTP_VERSION=22.2.2
# Tue, 14 Jan 2020 00:32:48 GMT
LABEL org.opencontainers.image.version=22.2.2
# Tue, 14 Jan 2020 00:49:05 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="92df7d22239b09f7580572305c862da1fb030a97cef7631ba060ac51fa3864cc" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 14 Jan 2020 00:49:06 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:8f0fdd3eaac017684c880d836abdaf02f9db7ac8ecca970356482e3d8e315650`  
		Last Modified: Sat, 28 Dec 2019 04:25:39 GMT  
		Size: 50.4 MB (50379720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:944f61469229e163a0ec073355db84ec450a7126f63ea96910dbc9ce2a3cea81`  
		Last Modified: Tue, 14 Jan 2020 01:10:53 GMT  
		Size: 59.4 MB (59373071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:058868963d24ba6bdb525dfc3557e2ddab1282cfaa627f52a3c715b1def4c1ba
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **101.0 MB (101010445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d3d4f147f18a5ca54caddb3c5e9612d8ce609e56c40e28880b4911edc32b7f9`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:58:42 GMT
ADD file:26fba5cd6ba1fe45f19fb80d1c8e54eac5189e2b93e521b2ba6d5a6b54175e81 in / 
# Sat, 28 Dec 2019 04:58:45 GMT
CMD ["bash"]
# Wed, 22 Jan 2020 01:07:39 GMT
ENV OTP_VERSION=22.2.3
# Wed, 22 Jan 2020 01:07:40 GMT
LABEL org.opencontainers.image.version=22.2.3
# Wed, 22 Jan 2020 01:14:13 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="8470fff519d9ffa5defba4e42c3c1e64cd86905313040246d4a6e35799a9e614" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 22 Jan 2020 01:14:16 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:760e5af4a2ec2472d42b6773d075af9d2a006e0b7725ba9992e530f561d326f8`  
		Last Modified: Sat, 28 Dec 2019 05:07:11 GMT  
		Size: 45.9 MB (45859628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7fbd03066a584e3e3cec2200a4549545dc9feeb17b606a08b0dfd32d93b3a0f`  
		Last Modified: Wed, 22 Jan 2020 02:12:02 GMT  
		Size: 55.2 MB (55150817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:e8c1491d56df606f02c4a5895ea602659b194f740133ddd73997c1457b7eabf2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.5 MB (105470441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:54aeaecb1813412a849e7994429afe46f43559ec71ea481dc3b8d07aaaafced7`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:40:41 GMT
ADD file:88b3d02fc98aa9138e694bee7d5d1b61b295e4a1c7fae399bf24e52eeff7a5ae in / 
# Sat, 28 Dec 2019 04:40:45 GMT
CMD ["bash"]
# Tue, 14 Jan 2020 00:49:49 GMT
ENV OTP_VERSION=22.2.2
# Tue, 14 Jan 2020 00:49:49 GMT
LABEL org.opencontainers.image.version=22.2.2
# Tue, 14 Jan 2020 00:56:44 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="92df7d22239b09f7580572305c862da1fb030a97cef7631ba060ac51fa3864cc" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 14 Jan 2020 00:56:46 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:627706d65d1d9b4038d8fd40db52238d4f11d9130a01f23ffae9bf5d41ac5933`  
		Last Modified: Sat, 28 Dec 2019 04:46:38 GMT  
		Size: 49.2 MB (49171876 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc14dc4e5759646fb27c8958a393846cdb9161cebb3eac0496fa8083eb210561`  
		Last Modified: Tue, 14 Jan 2020 01:05:45 GMT  
		Size: 56.3 MB (56298565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:slim` - linux; 386

```console
$ docker pull erlang@sha256:be02a387be6e5c0c3433ffc359488272b525bf744504be90e2079b18cd3f9d4a
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.9 MB (109878948 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb9743741d4378e0812a74ffaf91f50431c40db81f005bb39caf2b63afd6b443`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:20 GMT
ADD file:c2d3c2cbbc436161afbcdcab7f07d11962ae8a6e99f8ed2c4ff2bcc92455a406 in / 
# Sat, 28 Dec 2019 04:39:21 GMT
CMD ["bash"]
# Tue, 14 Jan 2020 01:04:23 GMT
ENV OTP_VERSION=22.2.2
# Tue, 14 Jan 2020 01:04:23 GMT
LABEL org.opencontainers.image.version=22.2.2
# Tue, 14 Jan 2020 01:18:52 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="92df7d22239b09f7580572305c862da1fb030a97cef7631ba060ac51fa3864cc" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 14 Jan 2020 01:18:52 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:b3ff5188aae7f0986a4e7385f8249878f585ef70be99706b3262795514448afc`  
		Last Modified: Sat, 28 Dec 2019 04:44:08 GMT  
		Size: 51.1 MB (51141961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63e86ec0fd0596eecddabe488bdf050ab8dacac1fc029b6801cde2007ee49635`  
		Last Modified: Tue, 14 Jan 2020 01:36:42 GMT  
		Size: 58.7 MB (58736987 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:slim` - linux; ppc64le

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

### `erlang:slim` - linux; s390x

```console
$ docker pull erlang@sha256:34d1839b084212827144f9b8c02e823d8d443a0606ff760e5379bd95061cc07c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.3 MB (105276796 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e81ffa4bddb238d3ef97d065a948d29fd08d684bb6ba230bb3da9bf0d65b395`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:51 GMT
ADD file:aeaf0b11195b2ba7eb7890ce128ad93c114a8e183a516cf2e4ea42da324c57ea in / 
# Sat, 28 Dec 2019 04:41:51 GMT
CMD ["bash"]
# Wed, 22 Jan 2020 01:46:34 GMT
ENV OTP_VERSION=22.2.3
# Wed, 22 Jan 2020 01:46:34 GMT
LABEL org.opencontainers.image.version=22.2.3
# Wed, 22 Jan 2020 01:50:43 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="8470fff519d9ffa5defba4e42c3c1e64cd86905313040246d4a6e35799a9e614" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 22 Jan 2020 01:50:43 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:3596c5a237f76c32832c1879a3d0c763989cb13fac0024673b03e9b549b868ea`  
		Last Modified: Sat, 28 Dec 2019 04:44:54 GMT  
		Size: 49.0 MB (48954508 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4a6252e6c565e9124cfd83531f9c19c4fd544365510e11a30e8008e89345d99`  
		Last Modified: Wed, 22 Jan 2020 02:25:25 GMT  
		Size: 56.3 MB (56322288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
