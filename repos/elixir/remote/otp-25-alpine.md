## `elixir:otp-25-alpine`

```console
$ docker pull elixir@sha256:1367d041241ab7bcb47e4ca77322837889790113884da993031bac3383e781af
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `elixir:otp-25-alpine` - linux; amd64

```console
$ docker pull elixir@sha256:2b0bc469fb68df9f067d89d552116966e1ca8348ed3dad8973cf2cdc569f17c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.3 MB (55322170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80cb983f89644327730a27f89dc002f8c099b9cb047e8240e52c0a0ec80ec6dc`
-	Default Command: `["iex"]`

```dockerfile
# Mon, 23 May 2022 19:19:30 GMT
ADD file:8e81116368669ed3dd361bc898d61bff249f524139a239fdaf3ec46869a39921 in / 
# Mon, 23 May 2022 19:19:31 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 18:44:16 GMT
ENV OTP_VERSION=25.0.3 REBAR3_VERSION=3.18.0
# Mon, 18 Jul 2022 18:44:16 GMT
LABEL org.opencontainers.image.version=25.0.3
# Mon, 18 Jul 2022 18:49:35 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e8eca69b6bdaac9cc8f3e3177dd2913920513495ee83bdecf73af546768febd6" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& apk add --no-cache --virtual .fetch-deps 		curl 		ca-certificates 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& apk add --no-cache --virtual .build-deps 		dpkg-dev dpkg 		gcc 		g++ 		libc-dev 		linux-headers 		make 		autoconf 		ncurses-dev 		openssl-dev 		unixodbc-dev 		lksctp-tools-dev 		tar 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(getconf _NPROCESSORS_ONLN) 	  && make install ) 	&& rm -rf $ERL_TOP 	&& find /usr/local -regex '/usr/local/lib/erlang/\(lib/\|erts-\).*/\(man\|doc\|obj\|c_src\|emacs\|info\|examples\)' | xargs rm -rf 	&& find /usr/local -name src | xargs -r find | grep -v '\.hrl$' | xargs rm -v || true 	&& find /usr/local -name src | xargs -r find | xargs rmdir -vp || true 	&& scanelf --nobanner -E ET_EXEC -BF '%F' --recursive /usr/local | xargs -r strip --strip-all 	&& scanelf --nobanner -E ET_DYN -BF '%F' --recursive /usr/local | xargs -r strip --strip-unneeded 	&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "${REBAR3_DOWNLOAD_SHA256}  rebar3-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/rebar3-src 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apk add --virtual .erlang-rundeps 		$runDeps 		lksctp-tools 		ca-certificates 	&& apk del .fetch-deps .build-deps
# Mon, 18 Jul 2022 18:49:35 GMT
CMD ["erl"]
# Mon, 18 Jul 2022 20:44:15 GMT
ENV ELIXIR_VERSION=v1.13.4 LANG=C.UTF-8
# Mon, 18 Jul 2022 20:45:04 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="95daf2dd3052e6ca7d4d849457eaaba09de52d65ca38d6933c65bc1cdf6b8579" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apk add --no-cache --virtual .build-deps $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apk del .build-deps
# Mon, 18 Jul 2022 20:45:05 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:2408cc74d12b6cd092bb8b516ba7d5e290f485d3eb9672efc00f0583730179e8`  
		Last Modified: Mon, 23 May 2022 19:09:38 GMT  
		Size: 2.8 MB (2798889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fafd370e100b0c00e8b908b4994f779e62d58895112d212ff12d2b46ee51ecea`  
		Last Modified: Mon, 18 Jul 2022 19:19:20 GMT  
		Size: 46.5 MB (46543939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e418caef8534da43b97d137e2176cf67fe16e82564e5b75939eaa46dc673f18b`  
		Last Modified: Mon, 18 Jul 2022 20:53:53 GMT  
		Size: 6.0 MB (5979342 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:otp-25-alpine` - linux; arm variant v7

```console
$ docker pull elixir@sha256:129cda01e82efbb2c39b7c2905059aa1fb58839aa3d6b9363c44a771e4d235b0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.8 MB (52781147 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65890fcd5da007161128186c2c62a0ac875a3bbf59d880630bf45a3b1b313062`
-	Default Command: `["iex"]`

```dockerfile
# Mon, 23 May 2022 18:57:46 GMT
ADD file:72698cc08524b911ebaacf992490707e5a951ddd2fe6edb3fb598e9dc7155049 in / 
# Mon, 23 May 2022 18:57:47 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 18:20:03 GMT
ENV OTP_VERSION=25.0.3 REBAR3_VERSION=3.18.0
# Mon, 18 Jul 2022 18:20:04 GMT
LABEL org.opencontainers.image.version=25.0.3
# Mon, 18 Jul 2022 18:28:07 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e8eca69b6bdaac9cc8f3e3177dd2913920513495ee83bdecf73af546768febd6" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& apk add --no-cache --virtual .fetch-deps 		curl 		ca-certificates 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& apk add --no-cache --virtual .build-deps 		dpkg-dev dpkg 		gcc 		g++ 		libc-dev 		linux-headers 		make 		autoconf 		ncurses-dev 		openssl-dev 		unixodbc-dev 		lksctp-tools-dev 		tar 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(getconf _NPROCESSORS_ONLN) 	  && make install ) 	&& rm -rf $ERL_TOP 	&& find /usr/local -regex '/usr/local/lib/erlang/\(lib/\|erts-\).*/\(man\|doc\|obj\|c_src\|emacs\|info\|examples\)' | xargs rm -rf 	&& find /usr/local -name src | xargs -r find | grep -v '\.hrl$' | xargs rm -v || true 	&& find /usr/local -name src | xargs -r find | xargs rmdir -vp || true 	&& scanelf --nobanner -E ET_EXEC -BF '%F' --recursive /usr/local | xargs -r strip --strip-all 	&& scanelf --nobanner -E ET_DYN -BF '%F' --recursive /usr/local | xargs -r strip --strip-unneeded 	&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "${REBAR3_DOWNLOAD_SHA256}  rebar3-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/rebar3-src 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apk add --virtual .erlang-rundeps 		$runDeps 		lksctp-tools 		ca-certificates 	&& apk del .fetch-deps .build-deps
# Mon, 18 Jul 2022 18:28:08 GMT
CMD ["erl"]
# Mon, 18 Jul 2022 20:55:32 GMT
ENV ELIXIR_VERSION=v1.13.4 LANG=C.UTF-8
# Mon, 18 Jul 2022 20:57:50 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="95daf2dd3052e6ca7d4d849457eaaba09de52d65ca38d6933c65bc1cdf6b8579" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apk add --no-cache --virtual .build-deps $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apk del .build-deps
# Mon, 18 Jul 2022 20:57:51 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:6366ba92f08e2418e90171f1e34bd86ecd50fdc95953b3f33b8943c143518eca`  
		Last Modified: Mon, 23 May 2022 18:59:17 GMT  
		Size: 2.4 MB (2411648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20038862e9095371137d3316281b767b11409f973fd55555c897c90e6636ad2`  
		Last Modified: Mon, 18 Jul 2022 19:28:04 GMT  
		Size: 44.4 MB (44390111 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a04c26db07c156e65e6dae82e526d59cce7c2da5940bbe8236a3e19e690848a`  
		Last Modified: Mon, 18 Jul 2022 21:21:56 GMT  
		Size: 6.0 MB (5979388 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:otp-25-alpine` - linux; arm64 variant v8

```console
$ docker pull elixir@sha256:7d677099ef48fce016ee54e813456b19caecd39517f6009f497dcfd9dbe98d07
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **54.9 MB (54863849 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d9a54cc06d254f3ed43e3a90fa68e19507473e446ff306ae0efaa64b802833e`
-	Default Command: `["iex"]`

```dockerfile
# Mon, 23 May 2022 19:39:22 GMT
ADD file:3ae36c6c4a1fc43157692da97c6c4fa6c3d0189ba82e2bef7f5aaf4a5e083f18 in / 
# Mon, 23 May 2022 19:39:22 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 17:57:26 GMT
ENV OTP_VERSION=25.0.3 REBAR3_VERSION=3.18.0
# Mon, 18 Jul 2022 17:57:27 GMT
LABEL org.opencontainers.image.version=25.0.3
# Mon, 18 Jul 2022 18:01:57 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e8eca69b6bdaac9cc8f3e3177dd2913920513495ee83bdecf73af546768febd6" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& apk add --no-cache --virtual .fetch-deps 		curl 		ca-certificates 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& apk add --no-cache --virtual .build-deps 		dpkg-dev dpkg 		gcc 		g++ 		libc-dev 		linux-headers 		make 		autoconf 		ncurses-dev 		openssl-dev 		unixodbc-dev 		lksctp-tools-dev 		tar 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(getconf _NPROCESSORS_ONLN) 	  && make install ) 	&& rm -rf $ERL_TOP 	&& find /usr/local -regex '/usr/local/lib/erlang/\(lib/\|erts-\).*/\(man\|doc\|obj\|c_src\|emacs\|info\|examples\)' | xargs rm -rf 	&& find /usr/local -name src | xargs -r find | grep -v '\.hrl$' | xargs rm -v || true 	&& find /usr/local -name src | xargs -r find | xargs rmdir -vp || true 	&& scanelf --nobanner -E ET_EXEC -BF '%F' --recursive /usr/local | xargs -r strip --strip-all 	&& scanelf --nobanner -E ET_DYN -BF '%F' --recursive /usr/local | xargs -r strip --strip-unneeded 	&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "${REBAR3_DOWNLOAD_SHA256}  rebar3-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/rebar3-src 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apk add --virtual .erlang-rundeps 		$runDeps 		lksctp-tools 		ca-certificates 	&& apk del .fetch-deps .build-deps
# Mon, 18 Jul 2022 18:01:57 GMT
CMD ["erl"]
# Mon, 18 Jul 2022 19:53:25 GMT
ENV ELIXIR_VERSION=v1.13.4 LANG=C.UTF-8
# Mon, 18 Jul 2022 19:54:07 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="95daf2dd3052e6ca7d4d849457eaaba09de52d65ca38d6933c65bc1cdf6b8579" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apk add --no-cache --virtual .build-deps $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apk del .build-deps
# Mon, 18 Jul 2022 19:54:08 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:b3c136eddcbf2003d3180787cef00f39d46b9fd9e4623178282ad6a8d63ad3b0`  
		Last Modified: Mon, 23 May 2022 19:08:34 GMT  
		Size: 2.7 MB (2694464 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5ef2cfced3093c5faf679f7aef54cd043ebfbe57468227856dc0abfcd608fe9`  
		Last Modified: Mon, 18 Jul 2022 18:27:57 GMT  
		Size: 46.2 MB (46189451 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2433bb808d8a720431a4451a5532099f0a242f2a550ca1270e832ed51e9493f`  
		Last Modified: Mon, 18 Jul 2022 20:04:23 GMT  
		Size: 6.0 MB (5979934 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:otp-25-alpine` - linux; 386

```console
$ docker pull elixir@sha256:3620beb29e468cd1cfeafca238e934bc19732abab9446300c1b4f6ce2efd33bb
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.9 MB (52914340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fb95458e9f8e86a9ddfa837b182d2de48b7e49101789416973ee07946a6a5cf`
-	Default Command: `["iex"]`

```dockerfile
# Mon, 18 Jul 2022 20:38:19 GMT
ADD file:be69b7550bf861d8fb12bdbe1edf3a0d2519a6a4da61bd04858b6258ffbf48a7 in / 
# Mon, 18 Jul 2022 20:38:19 GMT
CMD ["/bin/sh"]
# Tue, 19 Jul 2022 00:56:26 GMT
ENV OTP_VERSION=25.0.3 REBAR3_VERSION=3.18.0
# Tue, 19 Jul 2022 00:56:27 GMT
LABEL org.opencontainers.image.version=25.0.3
# Tue, 19 Jul 2022 01:01:53 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e8eca69b6bdaac9cc8f3e3177dd2913920513495ee83bdecf73af546768febd6" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& apk add --no-cache --virtual .fetch-deps 		curl 		ca-certificates 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& apk add --no-cache --virtual .build-deps 		dpkg-dev dpkg 		gcc 		g++ 		libc-dev 		linux-headers 		make 		autoconf 		ncurses-dev 		openssl-dev 		unixodbc-dev 		lksctp-tools-dev 		tar 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(getconf _NPROCESSORS_ONLN) 	  && make install ) 	&& rm -rf $ERL_TOP 	&& find /usr/local -regex '/usr/local/lib/erlang/\(lib/\|erts-\).*/\(man\|doc\|obj\|c_src\|emacs\|info\|examples\)' | xargs rm -rf 	&& find /usr/local -name src | xargs -r find | grep -v '\.hrl$' | xargs rm -v || true 	&& find /usr/local -name src | xargs -r find | xargs rmdir -vp || true 	&& scanelf --nobanner -E ET_EXEC -BF '%F' --recursive /usr/local | xargs -r strip --strip-all 	&& scanelf --nobanner -E ET_DYN -BF '%F' --recursive /usr/local | xargs -r strip --strip-unneeded 	&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "${REBAR3_DOWNLOAD_SHA256}  rebar3-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/rebar3-src 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apk add --virtual .erlang-rundeps 		$runDeps 		lksctp-tools 		ca-certificates 	&& apk del .fetch-deps .build-deps
# Tue, 19 Jul 2022 01:01:53 GMT
CMD ["erl"]
# Tue, 19 Jul 2022 03:47:33 GMT
ENV ELIXIR_VERSION=v1.13.4 LANG=C.UTF-8
# Tue, 19 Jul 2022 03:48:51 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="95daf2dd3052e6ca7d4d849457eaaba09de52d65ca38d6933c65bc1cdf6b8579" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apk add --no-cache --virtual .build-deps $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apk del .build-deps
# Tue, 19 Jul 2022 03:48:51 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:5d7f927419794ebb7496ac38b0659686317b2d2fac7252a4a0d40d43d5fdd662`  
		Last Modified: Mon, 18 Jul 2022 19:09:22 GMT  
		Size: 2.8 MB (2802334 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d667a3aaf59658c877a7a7c24963d28b627ae5fbf9acab44d6a7aee35017c14`  
		Last Modified: Tue, 19 Jul 2022 01:22:11 GMT  
		Size: 44.1 MB (44132011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5c66d488493cf3e8bb22b19d9c1602afdb315ff56f9e180580f0dae887cc40c`  
		Last Modified: Tue, 19 Jul 2022 03:59:10 GMT  
		Size: 6.0 MB (5979995 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:otp-25-alpine` - linux; ppc64le

```console
$ docker pull elixir@sha256:677e5c98194dad2a8fc99902e6eff7cc22df70a9e5d9dfb15316a615e2018422
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.0 MB (52967919 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0b2c4f205b751735cfc20186907edb6eeecde0cb9609c863b4b38c209bbd4a9`
-	Default Command: `["iex"]`

```dockerfile
# Mon, 18 Jul 2022 21:29:30 GMT
ADD file:69e4080f15f54e2d8f8aa25fdcba9c01dde149d43592edd5023106675e54a769 in / 
# Mon, 18 Jul 2022 21:29:31 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 21:31:30 GMT
ENV OTP_VERSION=25.0.3 REBAR3_VERSION=3.18.0
# Mon, 18 Jul 2022 21:31:32 GMT
LABEL org.opencontainers.image.version=25.0.3
# Mon, 18 Jul 2022 21:39:25 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e8eca69b6bdaac9cc8f3e3177dd2913920513495ee83bdecf73af546768febd6" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& apk add --no-cache --virtual .fetch-deps 		curl 		ca-certificates 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& apk add --no-cache --virtual .build-deps 		dpkg-dev dpkg 		gcc 		g++ 		libc-dev 		linux-headers 		make 		autoconf 		ncurses-dev 		openssl-dev 		unixodbc-dev 		lksctp-tools-dev 		tar 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(getconf _NPROCESSORS_ONLN) 	  && make install ) 	&& rm -rf $ERL_TOP 	&& find /usr/local -regex '/usr/local/lib/erlang/\(lib/\|erts-\).*/\(man\|doc\|obj\|c_src\|emacs\|info\|examples\)' | xargs rm -rf 	&& find /usr/local -name src | xargs -r find | grep -v '\.hrl$' | xargs rm -v || true 	&& find /usr/local -name src | xargs -r find | xargs rmdir -vp || true 	&& scanelf --nobanner -E ET_EXEC -BF '%F' --recursive /usr/local | xargs -r strip --strip-all 	&& scanelf --nobanner -E ET_DYN -BF '%F' --recursive /usr/local | xargs -r strip --strip-unneeded 	&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "${REBAR3_DOWNLOAD_SHA256}  rebar3-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/rebar3-src 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apk add --virtual .erlang-rundeps 		$runDeps 		lksctp-tools 		ca-certificates 	&& apk del .fetch-deps .build-deps
# Mon, 18 Jul 2022 21:39:28 GMT
CMD ["erl"]
# Mon, 18 Jul 2022 22:33:34 GMT
ENV ELIXIR_VERSION=v1.13.4 LANG=C.UTF-8
# Mon, 18 Jul 2022 22:35:58 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="95daf2dd3052e6ca7d4d849457eaaba09de52d65ca38d6933c65bc1cdf6b8579" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apk add --no-cache --virtual .build-deps $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apk del .build-deps
# Mon, 18 Jul 2022 22:36:03 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:602896d442490cd3fbb6599f0f862d3673b7cd58eca3ac842b8e09bf8d012443`  
		Last Modified: Mon, 18 Jul 2022 19:09:09 GMT  
		Size: 2.8 MB (2789923 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8fdd744a863db353900e97f3c50b7cb5941dffa622566589dd42699f5f508918`  
		Last Modified: Mon, 18 Jul 2022 22:07:41 GMT  
		Size: 44.2 MB (44198543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8a6f4a4b47eca232a65aacad829129a26ae09f0e304492ce422a93e5d14c402`  
		Last Modified: Mon, 18 Jul 2022 23:00:56 GMT  
		Size: 6.0 MB (5979453 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `elixir:otp-25-alpine` - linux; s390x

```console
$ docker pull elixir@sha256:34195a0f4f87a7baf073bc67fd16cf1d30dc0e65a3b00eecd431f2d25a21f89d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53125094 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12a610a15653dc1e836995a09cb2b49409134aa02237c491315f4dfaf4829459`
-	Default Command: `["iex"]`

```dockerfile
# Mon, 23 May 2022 19:41:59 GMT
ADD file:e1852d8ef555a0d3ef6d0b74a898720c82bb9f491430b06a0dd0499497ce118e in / 
# Mon, 23 May 2022 19:42:10 GMT
CMD ["/bin/sh"]
# Mon, 18 Jul 2022 18:29:19 GMT
ENV OTP_VERSION=25.0.3 REBAR3_VERSION=3.18.0
# Mon, 18 Jul 2022 18:29:19 GMT
LABEL org.opencontainers.image.version=25.0.3
# Mon, 18 Jul 2022 18:41:27 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="e8eca69b6bdaac9cc8f3e3177dd2913920513495ee83bdecf73af546768febd6" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& apk add --no-cache --virtual .fetch-deps 		curl 		ca-certificates 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& apk add --no-cache --virtual .build-deps 		dpkg-dev dpkg 		gcc 		g++ 		libc-dev 		linux-headers 		make 		autoconf 		ncurses-dev 		openssl-dev 		unixodbc-dev 		lksctp-tools-dev 		tar 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(getconf _NPROCESSORS_ONLN) 	  && make install ) 	&& rm -rf $ERL_TOP 	&& find /usr/local -regex '/usr/local/lib/erlang/\(lib/\|erts-\).*/\(man\|doc\|obj\|c_src\|emacs\|info\|examples\)' | xargs rm -rf 	&& find /usr/local -name src | xargs -r find | grep -v '\.hrl$' | xargs rm -v || true 	&& find /usr/local -name src | xargs -r find | xargs rmdir -vp || true 	&& scanelf --nobanner -E ET_EXEC -BF '%F' --recursive /usr/local | xargs -r strip --strip-all 	&& scanelf --nobanner -E ET_DYN -BF '%F' --recursive /usr/local | xargs -r strip --strip-unneeded 	&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "${REBAR3_DOWNLOAD_SHA256}  rebar3-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/rebar3-src 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apk add --virtual .erlang-rundeps 		$runDeps 		lksctp-tools 		ca-certificates 	&& apk del .fetch-deps .build-deps
# Mon, 18 Jul 2022 18:41:33 GMT
CMD ["erl"]
# Mon, 18 Jul 2022 20:17:15 GMT
ENV ELIXIR_VERSION=v1.13.4 LANG=C.UTF-8
# Mon, 18 Jul 2022 20:19:03 GMT
RUN set -xe 	&& ELIXIR_DOWNLOAD_URL="https://github.com/elixir-lang/elixir/archive/${ELIXIR_VERSION}.tar.gz" 	&& ELIXIR_DOWNLOAD_SHA256="95daf2dd3052e6ca7d4d849457eaaba09de52d65ca38d6933c65bc1cdf6b8579" 	&& buildDeps=' 		ca-certificates 		curl 		make 	' 	&& apk add --no-cache --virtual .build-deps $buildDeps 	&& curl -fSL -o elixir-src.tar.gz $ELIXIR_DOWNLOAD_URL 	&& echo "$ELIXIR_DOWNLOAD_SHA256  elixir-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/local/src/elixir 	&& tar -xzC /usr/local/src/elixir --strip-components=1 -f elixir-src.tar.gz 	&& rm elixir-src.tar.gz 	&& cd /usr/local/src/elixir 	&& make install clean 	&& find /usr/local/src/elixir/ -type f -not -regex "/usr/local/src/elixir/lib/[^\/]*/lib.*" -exec rm -rf {} + 	&& find /usr/local/src/elixir/ -type d -depth -empty -delete 	&& apk del .build-deps
# Mon, 18 Jul 2022 20:19:04 GMT
CMD ["iex"]
```

-	Layers:
	-	`sha256:af1ac1a73384e058591d04d19bc05a06781cc32d52d4593b468d6cb95eda9858`  
		Last Modified: Mon, 23 May 2022 19:43:36 GMT  
		Size: 2.6 MB (2580494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f08a3571ea57ff1af9a765b66ff8855e6cb55b9b5964f8d80a08445f3fd1cd7a`  
		Last Modified: Mon, 18 Jul 2022 19:39:55 GMT  
		Size: 44.6 MB (44565233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2dbeca417a98c90bf230ce3ed203247de4e13d347839281f613a3ffed55ffb59`  
		Last Modified: Mon, 18 Jul 2022 20:32:15 GMT  
		Size: 6.0 MB (5979367 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
