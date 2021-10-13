## `erlang:18-slim`

```console
$ docker pull erlang@sha256:21a8a31cb02a35728d1fcc0efa7e6670693596b41363154d2dc47ffab23f3726
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `erlang:18-slim` - linux; amd64

```console
$ docker pull erlang@sha256:db689e84be6040bd6436a786203e7c45f3066d89a700430e2cd7d755ea4d1348
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114449023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d6192cd9c50e00ed1d257406cc4829ce7683fd781a00b1bbdb79dc6f42044db`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 12 Oct 2021 01:22:41 GMT
ADD file:084c8b3d38d578aa3910f3786b67b058962dbfdfd4a49d6e0201f2e91670873b in / 
# Tue, 12 Oct 2021 01:22:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 11:46:02 GMT
ENV OTP_VERSION=18.3.4.11
# Tue, 12 Oct 2021 11:56:06 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="94f84e8ca0db0dcadd3411fa7a05dd937142b6ae830255dc341c30b45261b01a" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.0.2 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl1.0-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" --enable-sctp 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 12 Oct 2021 11:56:07 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:2f0ef4316716c8b8925ba3665932f8bf2cef3b072d82de1aeb269d6b8b61b84c`  
		Last Modified: Tue, 12 Oct 2021 01:29:27 GMT  
		Size: 45.4 MB (45379651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b06f6e7de15a799fdfbd431c9b52329595c1f4f36c6995645785ab97b7c2361c`  
		Last Modified: Tue, 12 Oct 2021 12:00:53 GMT  
		Size: 69.1 MB (69069372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:18-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:a9fb11e1d70e9b87779a29a88acf02ad029a109c9ae9221cea9dbac649a0f6e9
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **105.7 MB (105723148 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb453ede89b7191faaeb4fd3407f4f543594585442ac51e77abcfacc7c152f54`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 12 Oct 2021 01:34:07 GMT
ADD file:eb5955ccd54a486767e85aeb1c03ffc6d8667b5476d0cf17b892ca407f1c8853 in / 
# Tue, 12 Oct 2021 01:34:08 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:03:07 GMT
ENV OTP_VERSION=18.3.4.11
# Tue, 12 Oct 2021 05:10:49 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="94f84e8ca0db0dcadd3411fa7a05dd937142b6ae830255dc341c30b45261b01a" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.0.2 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl1.0-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" --enable-sctp 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 12 Oct 2021 05:10:51 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:8e9db3616ec4491d75e6c28254ff2376f24900797e7c4cc464f36a0c502b111f`  
		Last Modified: Tue, 12 Oct 2021 01:51:20 GMT  
		Size: 42.1 MB (42119423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:688e9f7c332f2d78f9ba2fa7e5d498b2a2b2c3eafbf1e5cb8a457254f9916b53`  
		Last Modified: Tue, 12 Oct 2021 05:25:56 GMT  
		Size: 63.6 MB (63603725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:18-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:06b672b63cc708749327bdf99a0808829efee5311e9c76deecc42c8adca14413
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.1 MB (108118826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:032392dabbc90228548dc647a46bdfdca9684c85c4075a11e45e53700484a5be`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 12 Oct 2021 01:43:16 GMT
ADD file:33c2886dff8a69edd550eb69499bf01658d58e2eff405d4b5d4cd5d5be535faa in / 
# Tue, 12 Oct 2021 01:43:16 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 23:53:45 GMT
ENV OTP_VERSION=18.3.4.11
# Tue, 12 Oct 2021 23:57:15 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="94f84e8ca0db0dcadd3411fa7a05dd937142b6ae830255dc341c30b45261b01a" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.0.2 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl1.0-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" --enable-sctp 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 12 Oct 2021 23:57:16 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:cd2a530f50c2591d61de58d0e9cf724f6c5a2e1112456f38562e289732464c0c`  
		Last Modified: Tue, 12 Oct 2021 01:52:05 GMT  
		Size: 43.2 MB (43176697 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c447b05b59acfe6ba2fb723afa272112ee09f19e6f743d71132c77152a954d3`  
		Last Modified: Wed, 13 Oct 2021 00:08:44 GMT  
		Size: 64.9 MB (64942129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:18-slim` - linux; 386

```console
$ docker pull erlang@sha256:fc14bf0c284e0d0a1f00f0310ca2d03f9ba688ea3882a61b06400ba370602a6c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.8 MB (117839616 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb0f91f0c61c00139656b538acc8891f8a7fb76ba23f175411535b6da0344ae9`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 12 Oct 2021 01:42:19 GMT
ADD file:5a6f08cc731f24357c3702231256fb05eb0a97733779b2ace406ba3c9bf64baa in / 
# Tue, 12 Oct 2021 01:42:19 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:09:48 GMT
ENV OTP_VERSION=18.3.4.11
# Tue, 12 Oct 2021 09:17:02 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="94f84e8ca0db0dcadd3411fa7a05dd937142b6ae830255dc341c30b45261b01a" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.0.2 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl1.0-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" --enable-sctp 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 12 Oct 2021 09:17:03 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:d2ef4e90cca7406b4907a34e3571153fc56e3ecc9b2b5fdbb7787f22877cfec5`  
		Last Modified: Tue, 12 Oct 2021 01:51:58 GMT  
		Size: 46.1 MB (46097164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:991f5f8f77aa1ba8ea610040170f1c5dd83d87786fd8df27a1e5ed274c66951c`  
		Last Modified: Tue, 12 Oct 2021 09:30:12 GMT  
		Size: 71.7 MB (71742452 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
