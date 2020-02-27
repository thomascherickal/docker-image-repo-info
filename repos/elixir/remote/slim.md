## `elixir:slim`

```console
$ docker pull elixir@sha256:b53b891dac5e47ae04ff034867a703ceaa18584fab5f30aad921f27d7483c251
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
$ docker pull elixir@sha256:e3c98faa106a5a64cfc281155e40dabf7d4ae2080e2277ff844d9ee5ba10c17b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.0 MB (116994886 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:361cc289496f268fd9c40d7546b285e6204a28ce2ede1db652a81547ada8176c`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 26 Feb 2020 00:37:07 GMT
ADD file:e05e45c33042db4ec7f71a5952d65ee8cb3786dcd76fa7a990f48a2def1344e2 in / 
# Wed, 26 Feb 2020 00:37:07 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:40:17 GMT
ENV OTP_VERSION=22.2.7
# Wed, 26 Feb 2020 02:40:17 GMT
LABEL org.opencontainers.image.version=22.2.7
# Wed, 26 Feb 2020 03:01:01 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="29487837a2dd6e3184257cdec067cd3f5c0cd9517fbfb2ffc962589d46afbf75" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:01:01 GMT
CMD ["erl"]
# Thu, 27 Feb 2020 03:55:32 GMT
ENV ELIXIR_VERSION=v1.10.1 LANG=C.UTF-8
# Thu, 27 Feb 2020 03:56:58 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bf10dc5cb084382384d69cc26b4f670a3eb0a97a6491182f4dcf540457f06c07" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Thu, 27 Feb 2020 03:56:58 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:50e431f790939a2f924af65084cc9d39c3d3fb9ad2d57d183b7eadf86ea46992`  
		Last Modified: Wed, 26 Feb 2020 00:44:04 GMT  
		Size: 50.4 MB (50381971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a58b2864e036d3d6ba77cee6918d9364cd06c75b65e562abc238a419b117d9f`  
		Last Modified: Wed, 26 Feb 2020 05:29:42 GMT  
		Size: 59.4 MB (59389911 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:524838fb78bc09d6e3fd7060068d6fd2eed5c4f68bf08718d20796de6194c659`  
		Last Modified: Thu, 27 Feb 2020 04:11:08 GMT  
		Size: 7.2 MB (7223004 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; arm variant v7

```console
$ docker pull elixir@sha256:6911ecd2e35205490458abe890a84b8f2198326b048efe85e44918d8ad0b27e0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.2 MB (108244407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2d99a936c68f10a92ba2991b7099784dfbfe0f89fa3d32b635ddc37a1177507b`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 26 Feb 2020 00:50:58 GMT
ADD file:38fdfcc3155e437ce162aa0ed9dcdc5893b8145e2f3ede2858ed2187d79bf718 in / 
# Wed, 26 Feb 2020 00:51:08 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 02:51:42 GMT
ENV OTP_VERSION=22.2.7
# Wed, 26 Feb 2020 02:51:42 GMT
LABEL org.opencontainers.image.version=22.2.7
# Wed, 26 Feb 2020 02:58:01 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="29487837a2dd6e3184257cdec067cd3f5c0cd9517fbfb2ffc962589d46afbf75" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 26 Feb 2020 02:58:04 GMT
CMD ["erl"]
# Wed, 26 Feb 2020 22:46:05 GMT
ENV ELIXIR_VERSION=v1.10.1 LANG=C.UTF-8
# Wed, 26 Feb 2020 22:48:26 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bf10dc5cb084382384d69cc26b4f670a3eb0a97a6491182f4dcf540457f06c07" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 22:48:27 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:3182cf45068cd9734abd8e38dedbb9930ede35ee8c11376ca2684e86f9a1aa85`  
		Last Modified: Wed, 26 Feb 2020 01:07:03 GMT  
		Size: 45.9 MB (45862691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92487ccfb3946c9e5ba6eafe0d1f4a893ac87260490599bdce836f6d54fd0eb4`  
		Last Modified: Wed, 26 Feb 2020 04:24:30 GMT  
		Size: 55.2 MB (55159210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:37bb05523d8c06a630f354b7cd9e5e6f43e853936a1fef58440ace5349a68618`  
		Last Modified: Wed, 26 Feb 2020 23:11:11 GMT  
		Size: 7.2 MB (7222506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; arm64 variant v8

```console
$ docker pull elixir@sha256:7b8d0b079d1bb44c64d8a12501d9e6098ddce17ee7d259df599a1f467b131d0a
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.7 MB (112691595 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:53e889b577f071d6a7a4b356f61cca05ed5a6cf3f286eb162215b361960e9ec2`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 26 Feb 2020 00:46:17 GMT
ADD file:e3320653f0d517a6181aa46fb47407790018e2d8dee590005ffdbee3d04f72d4 in / 
# Wed, 26 Feb 2020 00:46:19 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 04:43:01 GMT
ENV OTP_VERSION=22.2.7
# Wed, 26 Feb 2020 04:43:02 GMT
LABEL org.opencontainers.image.version=22.2.7
# Wed, 26 Feb 2020 04:49:42 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="29487837a2dd6e3184257cdec067cd3f5c0cd9517fbfb2ffc962589d46afbf75" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 26 Feb 2020 04:49:43 GMT
CMD ["erl"]
# Wed, 26 Feb 2020 23:51:32 GMT
ENV ELIXIR_VERSION=v1.10.1 LANG=C.UTF-8
# Wed, 26 Feb 2020 23:54:05 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bf10dc5cb084382384d69cc26b4f670a3eb0a97a6491182f4dcf540457f06c07" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 23:54:06 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:77b067f4ec14d48dbc8cd83b7a46fbb5f21fe01ea8911db256cc0168a30c1f5b`  
		Last Modified: Wed, 26 Feb 2020 00:55:50 GMT  
		Size: 49.2 MB (49169974 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34c50b5ae78ad99f89df8ed8b1701a97098875251ece1b099d2b5b41d62e9ccd`  
		Last Modified: Wed, 26 Feb 2020 06:13:43 GMT  
		Size: 56.3 MB (56298818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:185b720f097e164e5a5fe5ff5eb2ab3ee42f16899eb1cb105914fab99d02fddb`  
		Last Modified: Thu, 27 Feb 2020 00:18:15 GMT  
		Size: 7.2 MB (7222803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; 386

```console
$ docker pull elixir@sha256:c2fe61011aa7223cdcd3a98feb2bc306ce63b8ba20335df3741421a7091bf9e9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **117.1 MB (117121274 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb7eefcd687795b2c105628f47664d781b1f15f5ac3ac91ec251468d9ec09584`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 26 Feb 2020 00:31:58 GMT
ADD file:1deff975480520310bf2c8d3708554d98c696f82689f0b67f9a834217c861803 in / 
# Wed, 26 Feb 2020 00:31:59 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 01:51:13 GMT
ENV OTP_VERSION=22.2.7
# Wed, 26 Feb 2020 01:51:13 GMT
LABEL org.opencontainers.image.version=22.2.7
# Wed, 26 Feb 2020 02:07:50 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="29487837a2dd6e3184257cdec067cd3f5c0cd9517fbfb2ffc962589d46afbf75" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 26 Feb 2020 02:07:51 GMT
CMD ["erl"]
# Wed, 26 Feb 2020 19:44:00 GMT
ENV ELIXIR_VERSION=v1.10.1 LANG=C.UTF-8
# Wed, 26 Feb 2020 19:45:40 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bf10dc5cb084382384d69cc26b4f670a3eb0a97a6491182f4dcf540457f06c07" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 19:45:40 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:9450e7c48681b3ba36935d4e7d891b4b180d4d223a6c938faacb41402857ebd3`  
		Last Modified: Wed, 26 Feb 2020 00:38:12 GMT  
		Size: 51.1 MB (51146129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19204bede81135de84311d1ee42080d4d429a864fe40e2a033cc63a653ba4736`  
		Last Modified: Wed, 26 Feb 2020 04:56:36 GMT  
		Size: 58.8 MB (58752312 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:335b3ee4d680394844da80765c4bd65827784b23d28154b47410df37e2777168`  
		Last Modified: Wed, 26 Feb 2020 20:01:54 GMT  
		Size: 7.2 MB (7222833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; ppc64le

```console
$ docker pull elixir@sha256:cf77f5e9952a294fa10ff56a44ddff0db972d323ec5bd172a8dab49db8f27a37
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **118.6 MB (118566043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ef6c4e87c861fa159b1bd8f24bfc3751ba4be96980071f16c84355d3baabcc82`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 26 Feb 2020 01:30:27 GMT
ADD file:b58865b3fd36d440998ef82e567179a9cd6b9ce0343d5e5a15a0b4f856f211c7 in / 
# Wed, 26 Feb 2020 01:30:35 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 06:17:33 GMT
ENV OTP_VERSION=22.2.7
# Wed, 26 Feb 2020 06:17:38 GMT
LABEL org.opencontainers.image.version=22.2.7
# Wed, 26 Feb 2020 06:28:33 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="29487837a2dd6e3184257cdec067cd3f5c0cd9517fbfb2ffc962589d46afbf75" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 26 Feb 2020 06:28:39 GMT
CMD ["erl"]
# Wed, 26 Feb 2020 21:54:38 GMT
ENV ELIXIR_VERSION=v1.10.1 LANG=C.UTF-8
# Wed, 26 Feb 2020 21:59:46 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bf10dc5cb084382384d69cc26b4f670a3eb0a97a6491182f4dcf540457f06c07" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 21:59:54 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:928614537d6dedbdf79cc24c5c56bf98c3ed88f9d91a9ec1105d2a133611b0fd`  
		Last Modified: Wed, 26 Feb 2020 01:49:54 GMT  
		Size: 54.1 MB (54138444 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d780b4855314fe7d513d282596bed0fb7c92f32b31972e51001109a78e38205`  
		Last Modified: Wed, 26 Feb 2020 06:50:44 GMT  
		Size: 57.2 MB (57203874 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b90558eacc804bb8c40954ab8890304e4c3b52cb8e1d8eabdb5e936b70d6d56`  
		Last Modified: Wed, 26 Feb 2020 22:20:44 GMT  
		Size: 7.2 MB (7223725 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:slim` - linux; s390x

```console
$ docker pull elixir@sha256:5b2ef1f24010c5c27e335a19bd90124f9e69cdea56e6e240b25e7cb742e6ed77
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112509982 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ad7cf93318989f7fccd7cb0027c5451795723b5132fb6e50738803ce24a7265b`
-	Default Command: `["iex"]`

```dockerfile
# Wed, 26 Feb 2020 00:42:32 GMT
ADD file:80536bfff518f6b425ad359b86a124f79ccdc82deb3e648f1746a7c87a1fcad0 in / 
# Wed, 26 Feb 2020 00:42:35 GMT
CMD ["bash"]
# Wed, 26 Feb 2020 03:45:31 GMT
ENV OTP_VERSION=22.2.7
# Wed, 26 Feb 2020 03:45:31 GMT
LABEL org.opencontainers.image.version=22.2.7
# Wed, 26 Feb 2020 03:53:16 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="29487837a2dd6e3184257cdec067cd3f5c0cd9517fbfb2ffc962589d46afbf75" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 26 Feb 2020 03:53:20 GMT
CMD ["erl"]
# Wed, 26 Feb 2020 10:37:52 GMT
ENV ELIXIR_VERSION=v1.10.1 LANG=C.UTF-8
# Wed, 26 Feb 2020 10:39:03 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="bf10dc5cb084382384d69cc26b4f670a3eb0a97a6491182f4dcf540457f06c07" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 26 Feb 2020 10:39:04 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:0a3603da42bb9e22573006a7f894b198954caeab529e2e041660e12c4fe62462`  
		Last Modified: Wed, 26 Feb 2020 00:47:26 GMT  
		Size: 49.0 MB (48958029 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d670f9a580a6de2cd3e7ce5fa803366c8462988b0cb552ffa8d435fd3ea2d3b`  
		Last Modified: Wed, 26 Feb 2020 04:26:26 GMT  
		Size: 56.3 MB (56329414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86d331815b4db9aa0318ed19ac579fcac590dfdc70bd9f5310afbf5a2090bee7`  
		Last Modified: Wed, 26 Feb 2020 10:46:04 GMT  
		Size: 7.2 MB (7222539 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
