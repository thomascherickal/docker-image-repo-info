## `elixir:slim`

```console
$ docker pull elixir@sha256:35281dd7dc56e86cdc47d283ef6d7d862cf20772f454f81788f8aa9c4ffeb6df
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
$ docker pull elixir@sha256:d9d979526b06b1724e5432a75c7aeb28397a29545e99435539cf1047a9b1f6ee
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.2 MB (117215922 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:05a0053045a14a256549b4085ebba67dc8ae4e93b2c017f89589f11a598c48e8`
-	Default Command: `["iex"]`

```dockerfile
# Tue, 13 Oct 2020 01:38:30 GMT
ADD file:6627ad39ea0cb9fcb212342326d14efaff51aece1fd0dc16d5bbcaa25d858622 in / 
# Tue, 13 Oct 2020 01:38:30 GMT
CMD ["bash"]
# Tue, 20 Oct 2020 21:33:15 GMT
ENV OTP_VERSION=22.3.4.12
# Tue, 20 Oct 2020 21:33:15 GMT
LABEL org.opencontainers.image.version=22.3.4.12
# Tue, 20 Oct 2020 21:49:26 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="5607b27169edb2c02806f21330a3d430c55f21580292743d25b29b678e951aaf" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 20 Oct 2020 21:49:26 GMT
CMD ["erl"]
# Tue, 20 Oct 2020 22:42:24 GMT
ENV ELIXIR_VERSION=v1.10.4 LANG=C.UTF-8
# Tue, 20 Oct 2020 22:43:52 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="8518c78f43fe36315dbe0d623823c2c1b7a025c114f3f4adbb48e04ef63f1d9f" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 20 Oct 2020 22:43:52 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:e4c3d3e4f7b024979a1c12daa4073f6353b2ba92d96418bc90451994927c9bff`  
		Last Modified: Tue, 13 Oct 2020 01:48:02 GMT  
		Size: 50.4 MB (50395978 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a3162d51c6b1fd667dfa868db230546ea8add19936edf38a49514ebc192e988`  
		Last Modified: Tue, 20 Oct 2020 22:11:46 GMT  
		Size: 59.6 MB (59577136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:502f211328ccec8e07f71ce59c88a18bf5fe15d65f1e8b9442d471b7ba2c2c84`  
		Last Modified: Tue, 20 Oct 2020 22:54:06 GMT  
		Size: 7.2 MB (7242808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; arm variant v7

```console
$ docker pull elixir@sha256:5056c4aefe224108f3201c9df47455598576d17867e6bae939d34e664ec25651
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.5 MB (108463654 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e1c9af899be07ffa5b916f6a88ff4bac1a42210e0942d23e4eca48db6558f20`
-	Default Command: `["iex"]`

```dockerfile
# Tue, 13 Oct 2020 00:59:02 GMT
ADD file:e03270d36cef8171f1f6303860ff31bb1c0eb10642b8173bfdfef9f77fa4f89c in / 
# Tue, 13 Oct 2020 00:59:04 GMT
CMD ["bash"]
# Tue, 20 Oct 2020 21:09:54 GMT
ENV OTP_VERSION=22.3.4.12
# Tue, 20 Oct 2020 21:09:55 GMT
LABEL org.opencontainers.image.version=22.3.4.12
# Tue, 20 Oct 2020 21:16:18 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="5607b27169edb2c02806f21330a3d430c55f21580292743d25b29b678e951aaf" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 20 Oct 2020 21:16:21 GMT
CMD ["erl"]
# Tue, 20 Oct 2020 21:43:41 GMT
ENV ELIXIR_VERSION=v1.10.4 LANG=C.UTF-8
# Tue, 20 Oct 2020 21:46:04 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="8518c78f43fe36315dbe0d623823c2c1b7a025c114f3f4adbb48e04ef63f1d9f" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 20 Oct 2020 21:46:06 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:5c0fdcca2cbb5e316a288f39c8c2006f45544568ea04623c036e0b1faa066bbe`  
		Last Modified: Tue, 13 Oct 2020 01:08:04 GMT  
		Size: 45.9 MB (45869258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cca5aae2b13169cb287ea9387f4efaa8c1b033e5254dca5d98c4cc411665b1ea`  
		Last Modified: Tue, 20 Oct 2020 21:24:54 GMT  
		Size: 55.4 MB (55351965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:340dcc2e6ada41f4d67b7fee5f3e0e9e1c02b9f76edd836fc86eabfb44bf9636`  
		Last Modified: Tue, 20 Oct 2020 22:02:09 GMT  
		Size: 7.2 MB (7242431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; arm64 variant v8

```console
$ docker pull elixir@sha256:ab9934555daf42b427a84dc3b27ab0d13a19b6ee71a80dd31d7f6aabe17b6d14
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.9 MB (112904042 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a99451ec2103177fb571a68344bb0ad6dcb783554c3e6857d7b807ba7ba2e73d`
-	Default Command: `["iex"]`

```dockerfile
# Tue, 13 Oct 2020 01:40:40 GMT
ADD file:7a9016f6c75910c392bbea2cb9e146d1eba3942cdfd666a44004c79951c5d46f in / 
# Tue, 13 Oct 2020 01:40:45 GMT
CMD ["bash"]
# Tue, 20 Oct 2020 21:49:14 GMT
ENV OTP_VERSION=22.3.4.12
# Tue, 20 Oct 2020 21:49:14 GMT
LABEL org.opencontainers.image.version=22.3.4.12
# Tue, 20 Oct 2020 21:55:34 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="5607b27169edb2c02806f21330a3d430c55f21580292743d25b29b678e951aaf" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 20 Oct 2020 21:55:38 GMT
CMD ["erl"]
# Tue, 20 Oct 2020 22:23:20 GMT
ENV ELIXIR_VERSION=v1.10.4 LANG=C.UTF-8
# Tue, 20 Oct 2020 22:25:47 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="8518c78f43fe36315dbe0d623823c2c1b7a025c114f3f4adbb48e04ef63f1d9f" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 20 Oct 2020 22:25:48 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:04aacb10cb67f5fa248646a0ac9f40af5a6d3b0dbef65505bb7766bed6bf4885`  
		Last Modified: Tue, 13 Oct 2020 01:47:53 GMT  
		Size: 49.2 MB (49175405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:146902994cabfd6823f58b13728f4217ed8b47fb2ff356e4a616b45ff3d8bd38`  
		Last Modified: Tue, 20 Oct 2020 22:04:31 GMT  
		Size: 56.5 MB (56485972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1b2e62f0fcec1f260f60e09c6dbb5375d20abf8a47908081c3e3fa9c57e92e7`  
		Last Modified: Tue, 20 Oct 2020 22:41:27 GMT  
		Size: 7.2 MB (7242665 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; 386

```console
$ docker pull elixir@sha256:1ce6e4c46a4e512fbac8919c47ddcf05de9c492cc0965360dbe8ddaab4e46a2c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.3 MB (117337979 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7f806c1e48f1e86971c4995006fef4e11102b4c3b7b3706a98a97cd6b62362c6`
-	Default Command: `["iex"]`

```dockerfile
# Tue, 13 Oct 2020 01:40:35 GMT
ADD file:67b2b1e6cbc655edc4f78c724cd2048f8b0b336c3b56cca448b65ee9bb594ede in / 
# Tue, 13 Oct 2020 01:40:36 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 03:54:07 GMT
ENV OTP_VERSION=22.3.4.11
# Tue, 13 Oct 2020 03:54:07 GMT
LABEL org.opencontainers.image.version=22.3.4.11
# Tue, 13 Oct 2020 04:15:56 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="87a6ae1678d41c2a358bac7a2f4311ca37b6bdba6b239e85099c3a9bbb9d5d4d" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 13 Oct 2020 04:15:56 GMT
CMD ["erl"]
# Tue, 13 Oct 2020 21:35:34 GMT
ENV ELIXIR_VERSION=v1.10.4 LANG=C.UTF-8
# Tue, 13 Oct 2020 21:37:46 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="8518c78f43fe36315dbe0d623823c2c1b7a025c114f3f4adbb48e04ef63f1d9f" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 21:37:46 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:c303ed7c76e74ddfd5fc798c4922c89902a340db03b34bdaeb1974366f3c46a1`  
		Last Modified: Tue, 13 Oct 2020 01:48:38 GMT  
		Size: 51.2 MB (51158779 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7951162ff078ac89004a8873ab906384a358fe442474ce10583a802ac6110d91`  
		Last Modified: Tue, 13 Oct 2020 06:59:40 GMT  
		Size: 58.9 MB (58936564 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6637bedbf5eea09f180fca9dae09dc0d5e2eb8c9f3a0093d1860559eba9253d6`  
		Last Modified: Tue, 13 Oct 2020 21:56:35 GMT  
		Size: 7.2 MB (7242636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; ppc64le

```console
$ docker pull elixir@sha256:45cef43c6ecc4b611e64c850796254a8b8fbe01a2ba83d9779688c6e1d07ea2b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.8 MB (118774242 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:20d9b8d1163298cc0c4f3e62c3fbb3a86c3d2cd899e38d60232e05ac8301730f`
-	Default Command: `["iex"]`

```dockerfile
# Tue, 13 Oct 2020 01:37:39 GMT
ADD file:339c3116c875720e7ba27e67ec6c60bc913e8108f7cccce90537c0915c5130a5 in / 
# Tue, 13 Oct 2020 01:37:48 GMT
CMD ["bash"]
# Tue, 13 Oct 2020 02:32:11 GMT
ENV OTP_VERSION=22.3.4.11
# Tue, 13 Oct 2020 02:32:19 GMT
LABEL org.opencontainers.image.version=22.3.4.11
# Tue, 13 Oct 2020 02:47:45 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="87a6ae1678d41c2a358bac7a2f4311ca37b6bdba6b239e85099c3a9bbb9d5d4d" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 13 Oct 2020 02:47:53 GMT
CMD ["erl"]
# Tue, 13 Oct 2020 16:46:32 GMT
ENV ELIXIR_VERSION=v1.10.4 LANG=C.UTF-8
# Tue, 13 Oct 2020 16:50:25 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="8518c78f43fe36315dbe0d623823c2c1b7a025c114f3f4adbb48e04ef63f1d9f" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 13 Oct 2020 16:50:32 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:b5d2617265f370f18bc3d48beee684b1ba0eb6a2b02f813353f4bbd7084830ff`  
		Last Modified: Tue, 13 Oct 2020 01:49:15 GMT  
		Size: 54.1 MB (54142565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8776cede5a5ed2d1443709572eae7bc485de0e845489adfeea81c5dbc059dc87`  
		Last Modified: Tue, 13 Oct 2020 02:49:25 GMT  
		Size: 57.4 MB (57387971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9834194bac23412df33afdb67c6a2a1130b12a7e6a5572e60b292404e7950f3b`  
		Last Modified: Tue, 13 Oct 2020 16:57:27 GMT  
		Size: 7.2 MB (7243706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; s390x

```console
$ docker pull elixir@sha256:e6cea3cc22c90cc9d188034ecf2aa047fe79bdfd2d8058a028a275990fcad1ab
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.7 MB (112719904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a1cda400a45727059ff44ccd842c014d3f45ffb1f5514f18f5dfabd7e46ad829`
-	Default Command: `["iex"]`

```dockerfile
# Tue, 13 Oct 2020 01:42:06 GMT
ADD file:cc8968c8733f7fb6fb644b948e4a21999440d079560afbb2acb9d666de3886ec in / 
# Tue, 13 Oct 2020 01:42:09 GMT
CMD ["bash"]
# Tue, 20 Oct 2020 21:48:12 GMT
ENV OTP_VERSION=22.3.4.12
# Tue, 20 Oct 2020 21:48:12 GMT
LABEL org.opencontainers.image.version=22.3.4.12
# Tue, 20 Oct 2020 21:52:59 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="5607b27169edb2c02806f21330a3d430c55f21580292743d25b29b678e951aaf" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Tue, 20 Oct 2020 21:53:01 GMT
CMD ["erl"]
# Tue, 20 Oct 2020 22:16:43 GMT
ENV ELIXIR_VERSION=v1.10.4 LANG=C.UTF-8
# Tue, 20 Oct 2020 22:17:45 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="8518c78f43fe36315dbe0d623823c2c1b7a025c114f3f4adbb48e04ef63f1d9f" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Tue, 20 Oct 2020 22:17:46 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:dcbd85f88306d080bce94006a992947eaf462efa80b07c202b0514e6ef412fdf`  
		Last Modified: Tue, 13 Oct 2020 01:45:28 GMT  
		Size: 49.0 MB (48966292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e8c29a88db68069ce8c3fc4481aefde304bb085f298f1847964f7d157502450`  
		Last Modified: Tue, 20 Oct 2020 21:59:49 GMT  
		Size: 56.5 MB (56511251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:186b3b3102ee96b46270f7bd8eec2b4ce4f5dab13d7bec6f453f27d0f779cc02`  
		Last Modified: Tue, 20 Oct 2020 22:25:41 GMT  
		Size: 7.2 MB (7242361 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
