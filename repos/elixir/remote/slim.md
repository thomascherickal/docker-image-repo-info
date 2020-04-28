## `elixir:slim`

```console
$ docker pull elixir@sha256:9be109f280c5c11b82d78cf62c39745d4d1fc9eee8fde7f0ff0c1e7995866a67
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
$ docker pull elixir@sha256:19c1a21a7a718bd4c01afe0159dbda0e863f9b65d108b85cf8f6a7fe34b221e4
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.1 MB (117126994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b406cdc09952b92ac6d86f309a182d36737e673c61fc839a85aaa724425129a8`
-	Default Command: `["iex"]`

```dockerfile
# Thu, 23 Apr 2020 00:20:17 GMT
ADD file:f086177965196842af3c15f50a7f6ad7912aaa7bf73a60b1d00e3129265eec9a in / 
# Thu, 23 Apr 2020 00:20:17 GMT
CMD ["bash"]
# Mon, 27 Apr 2020 23:44:09 GMT
ENV OTP_VERSION=22.3.3
# Mon, 27 Apr 2020 23:44:09 GMT
LABEL org.opencontainers.image.version=22.3.3
# Tue, 28 Apr 2020 00:03:35 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="58ef3623cad5f490fdc0719514fe1a9626c8b177a4fb8fa25b5bec0216693eb9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 28 Apr 2020 00:03:35 GMT
CMD ["erl"]
# Tue, 28 Apr 2020 01:25:44 GMT
ENV ELIXIR_VERSION=v1.10.3 LANG=C.UTF-8
# Tue, 28 Apr 2020 01:27:15 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="f3035fc5fdade35c3592a5fa7c8ee1aadb736f565c46b74b68ed7828b3ee1897" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Apr 2020 01:27:15 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:90fe46dd819953eb995f9cc9c326130abe9dd0b3993a998e12c01d0218a0b831`  
		Last Modified: Thu, 23 Apr 2020 00:24:56 GMT  
		Size: 50.4 MB (50382927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14034bd64ba8afb22d5fa8a1b2767a6708534eba205fc30c2e6b25ac58301558`  
		Last Modified: Tue, 28 Apr 2020 01:22:26 GMT  
		Size: 59.5 MB (59514747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776257a6e4db212d8c64ca1c306bb612400f4a3e4acf3bd67bb73fb30f1e9493`  
		Last Modified: Tue, 28 Apr 2020 01:47:40 GMT  
		Size: 7.2 MB (7229320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; arm variant v7

```console
$ docker pull elixir@sha256:5f10c2dd9934720657e008c59651e80348306268a29fc0db289bedbcb6ac5333
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.4 MB (108380541 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8482a84357091eec426050a1bc26800e6b89f7c7011be54fa70c29cb5335b3f8`
-	Default Command: `["iex"]`

```dockerfile
# Thu, 23 Apr 2020 01:03:01 GMT
ADD file:67087d9a080132a9a5865637874fa3dab5059ac619630d071c563e75a7a5d977 in / 
# Thu, 23 Apr 2020 01:03:02 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:16:23 GMT
ENV OTP_VERSION=22.3.2
# Thu, 23 Apr 2020 03:16:23 GMT
LABEL org.opencontainers.image.version=22.3.2
# Thu, 23 Apr 2020 03:23:03 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4a3719c71a7998e4f57e73920439b4b1606f7c045e437a0f0f9f1613594d3eaa" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:23:06 GMT
CMD ["erl"]
# Mon, 27 Apr 2020 23:14:46 GMT
ENV ELIXIR_VERSION=v1.10.3 LANG=C.UTF-8
# Mon, 27 Apr 2020 23:18:35 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="f3035fc5fdade35c3592a5fa7c8ee1aadb736f565c46b74b68ed7828b3ee1897" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 27 Apr 2020 23:18:36 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:cb6703531d2fa1d357cdd21991ae844400ecd207dba47fdd9afad54cdd9ce65a`  
		Last Modified: Thu, 23 Apr 2020 01:10:47 GMT  
		Size: 45.9 MB (45864280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6a9486e041ee17e7690b4a5a275267e27e11923d05f7e42156c2a3a3d6d1e1e`  
		Last Modified: Thu, 23 Apr 2020 03:59:08 GMT  
		Size: 55.3 MB (55287296 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31aa2c096c30f151b05c5e8c04f6b4b749fc3caaac7bcee916807b41833dd139`  
		Last Modified: Mon, 27 Apr 2020 23:25:15 GMT  
		Size: 7.2 MB (7228965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; arm64 variant v8

```console
$ docker pull elixir@sha256:12beff97ca68017db9706a31e8065eb7801c286a40753553193962edfd596bd7
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.8 MB (112841924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84e49918cbd3e83620d4080adf149ab22231fbaccb9300125a4ce288243d06d8`
-	Default Command: `["iex"]`

```dockerfile
# Thu, 23 Apr 2020 00:54:22 GMT
ADD file:c49818672222185a0a985a8511744bd524fce453bddb137364d79a793dc5740f in / 
# Thu, 23 Apr 2020 00:54:26 GMT
CMD ["bash"]
# Mon, 27 Apr 2020 23:00:51 GMT
ENV OTP_VERSION=22.3.3
# Mon, 27 Apr 2020 23:00:53 GMT
LABEL org.opencontainers.image.version=22.3.3
# Mon, 27 Apr 2020 23:12:09 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="58ef3623cad5f490fdc0719514fe1a9626c8b177a4fb8fa25b5bec0216693eb9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Mon, 27 Apr 2020 23:12:12 GMT
CMD ["erl"]
# Tue, 28 Apr 2020 00:31:45 GMT
ENV ELIXIR_VERSION=v1.10.3 LANG=C.UTF-8
# Tue, 28 Apr 2020 00:34:15 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="f3035fc5fdade35c3592a5fa7c8ee1aadb736f565c46b74b68ed7828b3ee1897" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Apr 2020 00:34:17 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:6243ff87266a170a3ad584d6c9c13f9b93c3aa84bded170c0040480f6c4e4170`  
		Last Modified: Thu, 23 Apr 2020 01:03:05 GMT  
		Size: 49.2 MB (49169698 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d018b7c1dfbbc5254689466c2c2439b4a07a30a0aa4ccd6f3cf7b658b0c9100f`  
		Last Modified: Mon, 27 Apr 2020 23:55:43 GMT  
		Size: 56.4 MB (56443042 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7346c3c27114d7009464ab55785771ae93c9af04ce6194717166a0c9dae04133`  
		Last Modified: Tue, 28 Apr 2020 01:01:54 GMT  
		Size: 7.2 MB (7229184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; 386

```console
$ docker pull elixir@sha256:eea8852d70e5dabcfd489fb9aa1e8af8b87a2b584926d0d06e76883fbc05be52
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.3 MB (117267982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91d61f5cfcd9f03eab35e9bcd5c6e7e7e1fb9fee708a5f8d68ffd8e008476f6a`
-	Default Command: `["iex"]`

```dockerfile
# Thu, 23 Apr 2020 00:39:21 GMT
ADD file:10751e25934ebcf54b529ebd800a690886012d472846a404b452a1b27dc97eed in / 
# Thu, 23 Apr 2020 00:39:22 GMT
CMD ["bash"]
# Mon, 27 Apr 2020 23:00:09 GMT
ENV OTP_VERSION=22.3.3
# Mon, 27 Apr 2020 23:00:09 GMT
LABEL org.opencontainers.image.version=22.3.3
# Mon, 27 Apr 2020 23:12:47 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="58ef3623cad5f490fdc0719514fe1a9626c8b177a4fb8fa25b5bec0216693eb9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Mon, 27 Apr 2020 23:12:47 GMT
CMD ["erl"]
# Tue, 28 Apr 2020 01:29:32 GMT
ENV ELIXIR_VERSION=v1.10.3 LANG=C.UTF-8
# Tue, 28 Apr 2020 01:31:17 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="f3035fc5fdade35c3592a5fa7c8ee1aadb736f565c46b74b68ed7828b3ee1897" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 28 Apr 2020 01:31:17 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:5ca4f2c0deeb8dae824229454aa24e8d27bb031c4d3229fbc5465ac18d0fc46b`  
		Last Modified: Thu, 23 Apr 2020 00:44:20 GMT  
		Size: 51.1 MB (51147043 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a91b2509ae816ac46c087d9c0e9e74b94b77eb6dc421a90daecd59cd047798`  
		Last Modified: Tue, 28 Apr 2020 00:41:19 GMT  
		Size: 58.9 MB (58891879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eb8d66c7885db149b502982c790e7502e19c5676bdbf08aaa6945739a24d6ff1`  
		Last Modified: Tue, 28 Apr 2020 01:52:00 GMT  
		Size: 7.2 MB (7229060 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; ppc64le

```console
$ docker pull elixir@sha256:485514b0826eb55c1dd765f6e69978d468f3a9fcf9874258ae014313a4dfab29
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.7 MB (118706665 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7c59635ced8ba80a4412130ac6ab313214e743c8f18be1fdd29de1127f0c8243`
-	Default Command: `["iex"]`

```dockerfile
# Thu, 23 Apr 2020 00:34:50 GMT
ADD file:31369dd617691a0d7181117a065290be8cd8c32814e443ef0a7c7adf7e9d800a in / 
# Thu, 23 Apr 2020 00:34:54 GMT
CMD ["bash"]
# Thu, 23 Apr 2020 03:36:24 GMT
ENV OTP_VERSION=22.3.2
# Thu, 23 Apr 2020 03:36:26 GMT
LABEL org.opencontainers.image.version=22.3.2
# Thu, 23 Apr 2020 03:46:08 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4a3719c71a7998e4f57e73920439b4b1606f7c045e437a0f0f9f1613594d3eaa" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 23 Apr 2020 03:46:15 GMT
CMD ["erl"]
# Thu, 23 Apr 2020 18:03:02 GMT
ENV ELIXIR_VERSION=v1.10.2 LANG=C.UTF-8
# Thu, 23 Apr 2020 18:06:38 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="5adffcf4389aa82fcfbc84324ebbfa095fc657a0e15b2b055fc05184f96b2d50" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 23 Apr 2020 18:06:40 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:6bf15800932473d1ca0a2cca9bfac073da118f1172b9027f7e78394850b02d05`  
		Last Modified: Thu, 23 Apr 2020 00:49:32 GMT  
		Size: 54.1 MB (54139621 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd0e0a777d966302011f08e90c81fda99b2a28880a9575933000e390ae5122d3`  
		Last Modified: Thu, 23 Apr 2020 04:36:27 GMT  
		Size: 57.3 MB (57341774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1841752b87a429d7ae30325312d08ba7723f5660a783df56a036d65cbef60713`  
		Last Modified: Thu, 23 Apr 2020 18:37:29 GMT  
		Size: 7.2 MB (7225270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; s390x

```console
$ docker pull elixir@sha256:74dfb3eae325468842bb27eac1f9ac19106ddb7b175f4c19ef65f7a04afb623f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.7 MB (112656474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b5992fd07600684f2941f3e4792573fa69840110d1d2eb2bec1e7a62f1f52ff8`
-	Default Command: `["iex"]`

```dockerfile
# Thu, 23 Apr 2020 00:51:31 GMT
ADD file:ff6937c6922875bc0f7ac0b859b2943c2ac9f7b57ac747bae88cbf4e0d5d4848 in / 
# Thu, 23 Apr 2020 00:51:34 GMT
CMD ["bash"]
# Mon, 27 Apr 2020 22:49:28 GMT
ENV OTP_VERSION=22.3.3
# Mon, 27 Apr 2020 22:49:28 GMT
LABEL org.opencontainers.image.version=22.3.3
# Mon, 27 Apr 2020 22:54:49 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="58ef3623cad5f490fdc0719514fe1a9626c8b177a4fb8fa25b5bec0216693eb9" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Mon, 27 Apr 2020 22:54:52 GMT
CMD ["erl"]
# Mon, 27 Apr 2020 23:33:10 GMT
ENV ELIXIR_VERSION=v1.10.3 LANG=C.UTF-8
# Mon, 27 Apr 2020 23:34:36 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="f3035fc5fdade35c3592a5fa7c8ee1aadb736f565c46b74b68ed7828b3ee1897" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Mon, 27 Apr 2020 23:34:37 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:21544d2d1a0f1cb5666bb8ad68a1dd7dff9022d1f9e2e096808ab6ce5c4c9275`  
		Last Modified: Thu, 23 Apr 2020 00:55:45 GMT  
		Size: 49.0 MB (48960155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f71b79cdeaffe51348fb1755da4f2cc06b6307b68dbae707bae7cad23d7ba67`  
		Last Modified: Mon, 27 Apr 2020 23:21:00 GMT  
		Size: 56.5 MB (56467437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3d545b68cb616d8e998992ceecae12b11947a7c5f9aecc627b3402f5772ce6`  
		Last Modified: Mon, 27 Apr 2020 23:55:30 GMT  
		Size: 7.2 MB (7228882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
