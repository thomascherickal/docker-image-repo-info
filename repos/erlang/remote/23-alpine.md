## `erlang:23-alpine`

```console
$ docker pull erlang@sha256:591655e6eb36095c5b4c43609463d96a60469aaca20775e17edd2467dcae1d9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `erlang:23-alpine` - linux; amd64

```console
$ docker pull erlang@sha256:8060b8903b6d485bdee7dcccb7bc09c1321668569382c1a77e0ec5fd5e50a7b8
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45291652 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:12968ad2fcd703cd11933c8a77f4a1e5c5a11993b8cc8e1347d9ec6147fc2866`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 22:12:03 GMT
ENV OTP_VERSION=23.3.4.12 REBAR3_VERSION=3.18.0
# Thu, 24 Mar 2022 22:12:03 GMT
LABEL org.opencontainers.image.version=23.3.4.12
# Thu, 24 Mar 2022 22:19:18 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="823eaf8f93b40b977fd06c0b7bbb22e623e5bc9859a85e4ec6c34b2ba7d947d4" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& apk add --no-cache --virtual .fetch-deps 		curl 		ca-certificates 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& apk add --no-cache --virtual .build-deps 		dpkg-dev dpkg 		gcc 		g++ 		libc-dev 		linux-headers 		make 		autoconf 		ncurses-dev 		openssl-dev 		unixodbc-dev 		lksctp-tools-dev 		tar 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(getconf _NPROCESSORS_ONLN) 	  && make install ) 	&& rm -rf $ERL_TOP 	&& find /usr/local -regex '/usr/local/lib/erlang/\(lib/\|erts-\).*/\(man\|doc\|obj\|c_src\|emacs\|info\|examples\)' | xargs rm -rf 	&& find /usr/local -name src | xargs -r find | grep -v '\.hrl$' | xargs rm -v || true 	&& find /usr/local -name src | xargs -r find | xargs rmdir -vp || true 	&& scanelf --nobanner -E ET_EXEC -BF '%F' --recursive /usr/local | xargs -r strip --strip-all 	&& scanelf --nobanner -E ET_DYN -BF '%F' --recursive /usr/local | xargs -r strip --strip-unneeded 	&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "${REBAR3_DOWNLOAD_SHA256}  rebar3-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/rebar3-src 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apk add --virtual .erlang-rundeps 		$runDeps 		lksctp-tools 		ca-certificates 	&& apk del .fetch-deps .build-deps
# Thu, 24 Mar 2022 22:19:18 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:30ba2b2a49090077c79ecfb94392a2fd07e4bb19ea7578630ce256f6a738b904`  
		Last Modified: Thu, 24 Mar 2022 22:23:45 GMT  
		Size: 42.5 MB (42475483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-alpine` - linux; arm variant v7

```console
$ docker pull erlang@sha256:325b631cca872e92a952cc662cdcb200aab2f35d3fb45d80f6a3b9e336a76779
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.9 MB (43907125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bbcbe90579448116e4c88c59b4542a14d612b0a4f07df278e63ba79bef2ef4a3`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 17 Mar 2022 17:21:06 GMT
ADD file:c25fcf153ea349f64e08a1bd0756ce550f2a081ad56cc40c89027d85d1bc26da in / 
# Thu, 17 Mar 2022 17:21:06 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 21:55:03 GMT
ENV OTP_VERSION=23.3.4.12 REBAR3_VERSION=3.18.0
# Thu, 24 Mar 2022 21:55:03 GMT
LABEL org.opencontainers.image.version=23.3.4.12
# Thu, 24 Mar 2022 22:02:55 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="823eaf8f93b40b977fd06c0b7bbb22e623e5bc9859a85e4ec6c34b2ba7d947d4" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& apk add --no-cache --virtual .fetch-deps 		curl 		ca-certificates 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& apk add --no-cache --virtual .build-deps 		dpkg-dev dpkg 		gcc 		g++ 		libc-dev 		linux-headers 		make 		autoconf 		ncurses-dev 		openssl-dev 		unixodbc-dev 		lksctp-tools-dev 		tar 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(getconf _NPROCESSORS_ONLN) 	  && make install ) 	&& rm -rf $ERL_TOP 	&& find /usr/local -regex '/usr/local/lib/erlang/\(lib/\|erts-\).*/\(man\|doc\|obj\|c_src\|emacs\|info\|examples\)' | xargs rm -rf 	&& find /usr/local -name src | xargs -r find | grep -v '\.hrl$' | xargs rm -v || true 	&& find /usr/local -name src | xargs -r find | xargs rmdir -vp || true 	&& scanelf --nobanner -E ET_EXEC -BF '%F' --recursive /usr/local | xargs -r strip --strip-all 	&& scanelf --nobanner -E ET_DYN -BF '%F' --recursive /usr/local | xargs -r strip --strip-unneeded 	&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "${REBAR3_DOWNLOAD_SHA256}  rebar3-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/rebar3-src 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apk add --virtual .erlang-rundeps 		$runDeps 		lksctp-tools 		ca-certificates 	&& apk del .fetch-deps .build-deps
# Thu, 24 Mar 2022 22:02:56 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:c3a1157c36d8d156f7664fa098212ab2149a64bcb59767cdf4595a86617c17fd`  
		Last Modified: Thu, 17 Mar 2022 17:22:45 GMT  
		Size: 2.4 MB (2430456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5c54ba37a7defb901becd57bd1017afa86f2f706c154887b62e353788613b2a`  
		Last Modified: Thu, 24 Mar 2022 22:18:33 GMT  
		Size: 41.5 MB (41476669 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-alpine` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:5353e2f29ff7c74fd236cece6205d18863a889bef69b359b1725a0926ea53f4e
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.9 MB (44903313 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f31fb310820a479486370220ccda41e1b6b3d84d9737574714bbfb49c02ea411`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 22:08:06 GMT
ENV OTP_VERSION=23.3.4.12 REBAR3_VERSION=3.18.0
# Thu, 24 Mar 2022 22:08:07 GMT
LABEL org.opencontainers.image.version=23.3.4.12
# Thu, 24 Mar 2022 22:12:09 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="823eaf8f93b40b977fd06c0b7bbb22e623e5bc9859a85e4ec6c34b2ba7d947d4" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& apk add --no-cache --virtual .fetch-deps 		curl 		ca-certificates 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& apk add --no-cache --virtual .build-deps 		dpkg-dev dpkg 		gcc 		g++ 		libc-dev 		linux-headers 		make 		autoconf 		ncurses-dev 		openssl-dev 		unixodbc-dev 		lksctp-tools-dev 		tar 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(getconf _NPROCESSORS_ONLN) 	  && make install ) 	&& rm -rf $ERL_TOP 	&& find /usr/local -regex '/usr/local/lib/erlang/\(lib/\|erts-\).*/\(man\|doc\|obj\|c_src\|emacs\|info\|examples\)' | xargs rm -rf 	&& find /usr/local -name src | xargs -r find | grep -v '\.hrl$' | xargs rm -v || true 	&& find /usr/local -name src | xargs -r find | xargs rmdir -vp || true 	&& scanelf --nobanner -E ET_EXEC -BF '%F' --recursive /usr/local | xargs -r strip --strip-all 	&& scanelf --nobanner -E ET_DYN -BF '%F' --recursive /usr/local | xargs -r strip --strip-unneeded 	&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "${REBAR3_DOWNLOAD_SHA256}  rebar3-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/rebar3-src 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apk add --virtual .erlang-rundeps 		$runDeps 		lksctp-tools 		ca-certificates 	&& apk del .fetch-deps .build-deps
# Thu, 24 Mar 2022 22:12:10 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1aee276a123b6ad468d163317cc5a2d452a2ec08889c7c247118eaf2ff25ee09`  
		Last Modified: Thu, 24 Mar 2022 22:18:46 GMT  
		Size: 42.2 MB (42187425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-alpine` - linux; 386

```console
$ docker pull erlang@sha256:4675f01fc3c6c176d55a0bed4e554666d894be0eba60f442e7afdbeda396d8ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.3 MB (45289111 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:26254896a1381a4108df5a6e8fa54c7d2dcfbf8e977fc4249987203a670944fe`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 23 Mar 2022 14:59:36 GMT
ADD file:5bb8a2cf301e0add52528df0f7f5c5b3c9b14495c5aa85c8fd628731fcd348aa in / 
# Wed, 23 Mar 2022 14:59:36 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 22:11:09 GMT
ENV OTP_VERSION=23.3.4.12 REBAR3_VERSION=3.18.0
# Thu, 24 Mar 2022 22:11:10 GMT
LABEL org.opencontainers.image.version=23.3.4.12
# Thu, 24 Mar 2022 22:15:55 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="823eaf8f93b40b977fd06c0b7bbb22e623e5bc9859a85e4ec6c34b2ba7d947d4" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& apk add --no-cache --virtual .fetch-deps 		curl 		ca-certificates 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& apk add --no-cache --virtual .build-deps 		dpkg-dev dpkg 		gcc 		g++ 		libc-dev 		linux-headers 		make 		autoconf 		ncurses-dev 		openssl-dev 		unixodbc-dev 		lksctp-tools-dev 		tar 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(getconf _NPROCESSORS_ONLN) 	  && make install ) 	&& rm -rf $ERL_TOP 	&& find /usr/local -regex '/usr/local/lib/erlang/\(lib/\|erts-\).*/\(man\|doc\|obj\|c_src\|emacs\|info\|examples\)' | xargs rm -rf 	&& find /usr/local -name src | xargs -r find | grep -v '\.hrl$' | xargs rm -v || true 	&& find /usr/local -name src | xargs -r find | xargs rmdir -vp || true 	&& scanelf --nobanner -E ET_EXEC -BF '%F' --recursive /usr/local | xargs -r strip --strip-all 	&& scanelf --nobanner -E ET_DYN -BF '%F' --recursive /usr/local | xargs -r strip --strip-unneeded 	&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "${REBAR3_DOWNLOAD_SHA256}  rebar3-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/rebar3-src 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apk add --virtual .erlang-rundeps 		$runDeps 		lksctp-tools 		ca-certificates 	&& apk del .fetch-deps .build-deps
# Thu, 24 Mar 2022 22:15:55 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:8fd9b2c548e42517da6865245538c8f53b774738b4fd7cb2d57ad8716e71748c`  
		Last Modified: Thu, 17 Mar 2022 16:35:25 GMT  
		Size: 2.8 MB (2823782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cc4f69416b98e454ce4384cdbd5ef859ece4c7f74b4349d48911a56a7c2b7a1`  
		Last Modified: Thu, 24 Mar 2022 22:23:05 GMT  
		Size: 42.5 MB (42465329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-alpine` - linux; ppc64le

```console
$ docker pull erlang@sha256:f15d10d1cb76ad28f21f78e2a118e559915f6a83f28bf8f0eca4bfff6dbdcf8c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **45.4 MB (45386646 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1eb3c6bf326567888a44bd28d99eace93059b70d9aa3d899dc7e68b35b44043e`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 17 Mar 2022 18:18:43 GMT
ADD file:bf9c99d8209e0bed9fd3b62cbe691ebf3829d5a35e63e2b066f1f842577a6d24 in / 
# Thu, 17 Mar 2022 18:18:48 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 22:33:24 GMT
ENV OTP_VERSION=23.3.4.12 REBAR3_VERSION=3.18.0
# Thu, 24 Mar 2022 22:33:27 GMT
LABEL org.opencontainers.image.version=23.3.4.12
# Thu, 24 Mar 2022 22:42:30 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="823eaf8f93b40b977fd06c0b7bbb22e623e5bc9859a85e4ec6c34b2ba7d947d4" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& apk add --no-cache --virtual .fetch-deps 		curl 		ca-certificates 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& apk add --no-cache --virtual .build-deps 		dpkg-dev dpkg 		gcc 		g++ 		libc-dev 		linux-headers 		make 		autoconf 		ncurses-dev 		openssl-dev 		unixodbc-dev 		lksctp-tools-dev 		tar 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(getconf _NPROCESSORS_ONLN) 	  && make install ) 	&& rm -rf $ERL_TOP 	&& find /usr/local -regex '/usr/local/lib/erlang/\(lib/\|erts-\).*/\(man\|doc\|obj\|c_src\|emacs\|info\|examples\)' | xargs rm -rf 	&& find /usr/local -name src | xargs -r find | grep -v '\.hrl$' | xargs rm -v || true 	&& find /usr/local -name src | xargs -r find | xargs rmdir -vp || true 	&& scanelf --nobanner -E ET_EXEC -BF '%F' --recursive /usr/local | xargs -r strip --strip-all 	&& scanelf --nobanner -E ET_DYN -BF '%F' --recursive /usr/local | xargs -r strip --strip-unneeded 	&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "${REBAR3_DOWNLOAD_SHA256}  rebar3-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/rebar3-src 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apk add --virtual .erlang-rundeps 		$runDeps 		lksctp-tools 		ca-certificates 	&& apk del .fetch-deps .build-deps
# Thu, 24 Mar 2022 22:42:36 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:8b7e8363a93630a772b70e3cf72231f43c62addae0ee8e507c61d43e3781c4e7`  
		Last Modified: Thu, 17 Mar 2022 18:20:01 GMT  
		Size: 2.8 MB (2817281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7097c382cadd3da2ac891eceb1b42b30c9139fc13998e934ab4326c44009afa9`  
		Last Modified: Thu, 24 Mar 2022 22:50:10 GMT  
		Size: 42.6 MB (42569365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:23-alpine` - linux; s390x

```console
$ docker pull erlang@sha256:6777aec0933a9881667fd2aeef6969576c927ea416a1e726d3d44b2f8b863300
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.3 MB (44324245 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c232890497b647351b8a9c4efaff8bb303957f929af0a526e0d9d23256133fa1`
-	Default Command: `["erl"]`

```dockerfile
# Thu, 17 Mar 2022 14:35:54 GMT
ADD file:cd4f7409c75ce2e40b46bbdeca277e2c4500aab51e1a7b6fa518c60e371f0a33 in / 
# Thu, 17 Mar 2022 14:35:55 GMT
CMD ["/bin/sh"]
# Thu, 24 Mar 2022 22:08:51 GMT
ENV OTP_VERSION=23.3.4.12 REBAR3_VERSION=3.18.0
# Thu, 24 Mar 2022 22:08:51 GMT
LABEL org.opencontainers.image.version=23.3.4.12
# Thu, 24 Mar 2022 22:13:02 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="823eaf8f93b40b977fd06c0b7bbb22e623e5bc9859a85e4ec6c34b2ba7d947d4" 	&& REBAR3_DOWNLOAD_SHA256="cce1925d33240d81d0e4d2de2eef3616d4c17b0532ed004274f875e6607d25d2" 	&& apk add --no-cache --virtual .fetch-deps 		curl 		ca-certificates 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& apk add --no-cache --virtual .build-deps 		dpkg-dev dpkg 		gcc 		g++ 		libc-dev 		linux-headers 		make 		autoconf 		ncurses-dev 		openssl-dev 		unixodbc-dev 		lksctp-tools-dev 		tar 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(getconf _NPROCESSORS_ONLN) 	  && make install ) 	&& rm -rf $ERL_TOP 	&& find /usr/local -regex '/usr/local/lib/erlang/\(lib/\|erts-\).*/\(man\|doc\|obj\|c_src\|emacs\|info\|examples\)' | xargs rm -rf 	&& find /usr/local -name src | xargs -r find | grep -v '\.hrl$' | xargs rm -v || true 	&& find /usr/local -name src | xargs -r find | xargs rmdir -vp || true 	&& scanelf --nobanner -E ET_EXEC -BF '%F' --recursive /usr/local | xargs -r strip --strip-all 	&& scanelf --nobanner -E ET_DYN -BF '%F' --recursive /usr/local | xargs -r strip --strip-unneeded 	&& runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)" 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "${REBAR3_DOWNLOAD_SHA256}  rebar3-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/rebar3-src 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src 	&& apk add --virtual .erlang-rundeps 		$runDeps 		lksctp-tools 		ca-certificates 	&& apk del .fetch-deps .build-deps
# Thu, 24 Mar 2022 22:13:03 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:1a9a9eea18bd912112f7ed42a3730393bafbb84387ab6790fe9358d09100f3a3`  
		Last Modified: Thu, 17 Mar 2022 14:36:47 GMT  
		Size: 2.6 MB (2605208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:456695fc9295cf3cf4c4c5c9be81323e9f6b017fbc7d233eb4b43721263b3c66`  
		Last Modified: Thu, 24 Mar 2022 22:17:09 GMT  
		Size: 41.7 MB (41719037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
