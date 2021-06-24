## `erlang:latest`

```console
$ docker pull erlang@sha256:398a874f44127ca956f81713f22060caf51898c5d44efdc54adbe496af2b1cb6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `erlang:latest` - linux; amd64

```console
$ docker pull erlang@sha256:0b1ed52980d94d61ebaededad325d9a7d579ef6071d756a08800758aaa0713a1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **485.6 MB (485591289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2c73fee263f554bf1979832b330b95480cf7cc89e77e696fcddbefe6174062`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:25 GMT
ADD file:a232795a746e5842d1a864a00462be6bd86543aeed8d06d2830dd955a4c1b3fc in / 
# Wed, 23 Jun 2021 00:20:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:52:59 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:53:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:53:28 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:54:26 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 01:09:56 GMT
ENV OTP_VERSION=24.0.2 REBAR3_VERSION=3.16.1
# Wed, 23 Jun 2021 01:09:56 GMT
LABEL org.opencontainers.image.version=24.0.2
# Wed, 23 Jun 2021 01:27:53 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4abca2cda7fc962ad65575e5ed834dd69c745e7e637f92cfd49f384a281d0f18" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 23 Jun 2021 01:27:55 GMT
CMD ["erl"]
# Wed, 23 Jun 2021 01:27:56 GMT
ENV REBAR_VERSION=2.6.4
# Wed, 23 Jun 2021 01:27:59 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Wed, 23 Jun 2021 01:28:25 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="a14711b09f6e1fc1b080b79d78c304afebcbb7fafed9d0972eb739f0ed89121b" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
```

-	Layers:
	-	`sha256:0bc3020d05f1e08b41f1c5d54650a157b1690cde7fedb1fafbc9cda70ee2ec5c`  
		Last Modified: Wed, 23 Jun 2021 00:25:08 GMT  
		Size: 50.4 MB (50435617 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a110e58716600c199fc95f633b30735c33a25b5adcfb16d1d7edbcb78a3f1b62`  
		Last Modified: Wed, 23 Jun 2021 01:01:46 GMT  
		Size: 7.8 MB (7832997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d3c0fa203acbade733bff627daa75b84c97f9d0553bcdf967a3f1d37471277`  
		Last Modified: Wed, 23 Jun 2021 01:01:47 GMT  
		Size: 10.0 MB (9997255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8fd09c11b021b756b7a92a4f70a3d444ce7e63a1c24e5749d236dc2c6e68514`  
		Last Modified: Wed, 23 Jun 2021 01:02:12 GMT  
		Size: 51.8 MB (51841560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:14feb89c4a52c44f0a7e23a46ebb76e1c25c4b2915a39656a3ab634c74bcda46`  
		Last Modified: Wed, 23 Jun 2021 01:02:56 GMT  
		Size: 192.4 MB (192393721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0af3de17cb405dd1389bae1350adfdf3737210698c70e02139599ceacc7f1d16`  
		Last Modified: Wed, 23 Jun 2021 05:43:39 GMT  
		Size: 171.9 MB (171937758 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fd696287fce8746d46da0c5b32bc35be0a8c87d23daa5b014a37aa74ba85158`  
		Last Modified: Wed, 23 Jun 2021 05:43:11 GMT  
		Size: 196.5 KB (196522 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82eb4dccf8b234f66178df8649b689a9e34788da8f0d4e408973a214e171b2ea`  
		Last Modified: Wed, 23 Jun 2021 05:43:12 GMT  
		Size: 955.9 KB (955859 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:latest` - linux; arm variant v7

```console
$ docker pull erlang@sha256:d68ac1d97da6e517aefef20898b23ad7ce4df342193e25d0657751040853977d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **433.5 MB (433531387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7394fb69c5f865c6b0e4084c5703d26716a5f9857eba3a71e6379a6990698c78`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 23 Jun 2021 00:20:01 GMT
ADD file:3edc1a2322b55593b3cd8e935ca6d837e7618bcaaab27a09c9822728f8272ce0 in / 
# Wed, 23 Jun 2021 00:20:02 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 05:46:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:46:20 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 05:47:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 05:49:10 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 24 Jun 2021 08:27:47 GMT
ENV OTP_VERSION=24.0.2 REBAR3_VERSION=3.16.1
# Thu, 24 Jun 2021 08:27:47 GMT
LABEL org.opencontainers.image.version=24.0.2
# Thu, 24 Jun 2021 08:38:22 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4abca2cda7fc962ad65575e5ed834dd69c745e7e637f92cfd49f384a281d0f18" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Thu, 24 Jun 2021 08:38:23 GMT
CMD ["erl"]
# Thu, 24 Jun 2021 08:38:24 GMT
ENV REBAR_VERSION=2.6.4
# Thu, 24 Jun 2021 08:38:33 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Thu, 24 Jun 2021 08:39:17 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="a14711b09f6e1fc1b080b79d78c304afebcbb7fafed9d0972eb739f0ed89121b" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
```

-	Layers:
	-	`sha256:a3ac2852d9d20585eb4d19973a45b69522d16832456ea5b52f0298b2937afc09`  
		Last Modified: Wed, 23 Jun 2021 00:31:04 GMT  
		Size: 45.9 MB (45917482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d59952ec0a1da3155a9d9a84f07fc99163c3b5429cae2d6d37e9de664191d9d`  
		Last Modified: Wed, 23 Jun 2021 06:18:36 GMT  
		Size: 7.1 MB (7124226 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ac8017b9330d1a833e533de62b0525c9033b03c74f0d5c3b28b478231b03803`  
		Last Modified: Wed, 23 Jun 2021 06:18:37 GMT  
		Size: 9.3 MB (9343805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e065f215c483cb5ee70970d3a4708cdce964e110f4d6e1c6f19ff783e71842fb`  
		Last Modified: Wed, 23 Jun 2021 06:19:26 GMT  
		Size: 47.4 MB (47357244 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fb2edff8d52e8cba3157e63084f9fba762cbebd40aeadab6280a5a2a642cb49`  
		Last Modified: Wed, 23 Jun 2021 06:21:21 GMT  
		Size: 168.6 MB (168590645 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e6f98bf38202f411dea2873efe53adf29aa504628cd0ed859e61a7f3b9193d`  
		Last Modified: Thu, 24 Jun 2021 10:16:41 GMT  
		Size: 154.0 MB (154045580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:440fb5a0df31d9fa43498d6cc83e3a9489a97bf795159d64f04ea3ceda6dc575`  
		Last Modified: Thu, 24 Jun 2021 10:15:09 GMT  
		Size: 196.5 KB (196543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aef5d75273343c2822da5041b5348f05a90b14244cf3c968f833d3db7646781f`  
		Last Modified: Thu, 24 Jun 2021 10:15:09 GMT  
		Size: 955.9 KB (955862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:latest` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:1732eaf06fd8f15513bf52254e008d0284550d46f1ed0c56fd4d3dacace85d0c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **463.6 MB (463568456 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16168cf7af41b3e62e84b9b9a628befebae7c0748f67b5fbc5fdf62d147d3638`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 22 Jun 2021 23:49:24 GMT
ADD file:bc9eebfc439e3fbf9db01c98dc2448d9bededd394b893e397661227b81859dea in / 
# Tue, 22 Jun 2021 23:49:25 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:24:36 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:24:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:25:00 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:25:47 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:37:58 GMT
ENV OTP_VERSION=24.0.2 REBAR3_VERSION=3.16.1
# Wed, 23 Jun 2021 00:37:58 GMT
LABEL org.opencontainers.image.version=24.0.2
# Wed, 23 Jun 2021 00:45:28 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4abca2cda7fc962ad65575e5ed834dd69c745e7e637f92cfd49f384a281d0f18" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:45:29 GMT
CMD ["erl"]
# Wed, 23 Jun 2021 00:45:30 GMT
ENV REBAR_VERSION=2.6.4
# Wed, 23 Jun 2021 00:45:34 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Wed, 23 Jun 2021 00:46:01 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="a14711b09f6e1fc1b080b79d78c304afebcbb7fafed9d0972eb739f0ed89121b" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
```

-	Layers:
	-	`sha256:310b368da98207b4fd030cc969461bfba1ea7c73fc5da1f015e05570d3eb2510`  
		Last Modified: Tue, 22 Jun 2021 23:54:51 GMT  
		Size: 49.2 MB (49221986 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86422c44ee005c4d5ccb0e2fa32685229207b712728cd4b8c0ef97174f079df7`  
		Last Modified: Wed, 23 Jun 2021 00:33:16 GMT  
		Size: 7.7 MB (7694715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9137877e0c26a439a8954003b21876b6059de852c839631e8cf6fda5bd36434c`  
		Last Modified: Wed, 23 Jun 2021 00:33:17 GMT  
		Size: 10.0 MB (9984281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:785171b903c4d81c5b7539417a7b05f4a9bc6a35840595233bf4e369d8aee387`  
		Last Modified: Wed, 23 Jun 2021 00:33:41 GMT  
		Size: 52.2 MB (52165169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0373cebfde2cc9a301ad49bdd4883de5ab6dd6d5416932aa96428f70fac5000c`  
		Last Modified: Wed, 23 Jun 2021 00:34:23 GMT  
		Size: 184.0 MB (183974602 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b590efc6ace44ec18ea02e8c7965a64e0cc8134fab66ae6dc0990604af22b386`  
		Last Modified: Wed, 23 Jun 2021 02:24:13 GMT  
		Size: 159.4 MB (159375355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8535f8fb12f6ef849526a2fd58be4ead906b5a7f070b5820b38a364695738d63`  
		Last Modified: Wed, 23 Jun 2021 02:23:50 GMT  
		Size: 196.5 KB (196491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6793f4d1801952666bfbaac4b589ef53599ba11a92e89b62cda53d0ad7070da8`  
		Last Modified: Wed, 23 Jun 2021 02:23:50 GMT  
		Size: 955.9 KB (955857 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:latest` - linux; 386

```console
$ docker pull erlang@sha256:0ba3a623f76f103592bd0a5bdaaf7eb3484014c2d5f9ef2471ed5694e70d0c44
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **488.2 MB (488182370 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ae5b8e5be92adb01ac4ff7b5eb9e53e8801857fd551a7e0c5fcac6a3b27dcc46`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 22 Jun 2021 23:39:18 GMT
ADD file:e69bc1dee51190c812075d4b4e8ba1e67f67250af9f2ddbaecaf2c9316a07bbd in / 
# Tue, 22 Jun 2021 23:39:18 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:09:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:09:18 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:09:41 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:10:44 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:34:12 GMT
ENV OTP_VERSION=24.0.2 REBAR3_VERSION=3.16.1
# Wed, 23 Jun 2021 00:34:13 GMT
LABEL org.opencontainers.image.version=24.0.2
# Wed, 23 Jun 2021 00:44:44 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4abca2cda7fc962ad65575e5ed834dd69c745e7e637f92cfd49f384a281d0f18" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:44:45 GMT
CMD ["erl"]
# Wed, 23 Jun 2021 00:44:45 GMT
ENV REBAR_VERSION=2.6.4
# Wed, 23 Jun 2021 00:44:50 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Wed, 23 Jun 2021 00:45:16 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="a14711b09f6e1fc1b080b79d78c304afebcbb7fafed9d0972eb739f0ed89121b" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
```

-	Layers:
	-	`sha256:c4109247a8f9a72ed1435270480f72d6db8d6f038c6941d86a94f4dd0be8f789`  
		Last Modified: Tue, 22 Jun 2021 23:45:45 GMT  
		Size: 51.2 MB (51207098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:823a83541e8a9ed59943f9915ac65a73f57137e829772a16bc0bca5031a8cc07`  
		Last Modified: Wed, 23 Jun 2021 00:17:58 GMT  
		Size: 8.0 MB (7998521 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce7455379cfe2e69e9290d3b103e5889bee3e1c03187bb9e2a454325fd6a7f1a`  
		Last Modified: Wed, 23 Jun 2021 00:17:58 GMT  
		Size: 10.3 MB (10339805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:295349fcd02216e45784e329283de2e5811af98fafed9195ab2cf24bf58febe2`  
		Last Modified: Wed, 23 Jun 2021 00:18:25 GMT  
		Size: 53.4 MB (53436615 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15859f8c06830467d6c8e426b5b5e10d0c53a2a8a7cfb7899e7ef81badfd7ce`  
		Last Modified: Wed, 23 Jun 2021 00:19:13 GMT  
		Size: 198.9 MB (198933340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bac384c3091eb9435181a9e2e54b334a3424f2efaa8c0bc5531a0c795a96dc7a`  
		Last Modified: Wed, 23 Jun 2021 05:12:44 GMT  
		Size: 165.1 MB (165114644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae134849b96e65f232312aa68e653b1fe9e49df38ba001dddd9986a3ed2e81e9`  
		Last Modified: Wed, 23 Jun 2021 05:11:50 GMT  
		Size: 196.5 KB (196484 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53e79f5c05c267beb2d67302a4141ee9bc548525f8e09d177902ca7cd24b9508`  
		Last Modified: Wed, 23 Jun 2021 05:11:50 GMT  
		Size: 955.9 KB (955863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:latest` - linux; ppc64le

```console
$ docker pull erlang@sha256:cda81a1d5b425148815decb20f3cd476d2e6b45bef37df7dfaaf93cf8cf2d220
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **502.6 MB (502585348 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80c1992d15df689c0861b47a9b013ae762cfacdbcf480c76dd0a1bc799ce2282`
-	Default Command: `["erl"]`

```dockerfile
# Wed, 23 Jun 2021 00:30:05 GMT
ADD file:b73f8d66b8be6103349949991124c7d82e38589b2db6212e920cb3b6d5ceefef in / 
# Wed, 23 Jun 2021 00:30:13 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 02:33:41 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 02:34:44 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 02:38:20 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 02:52:19 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 19:11:08 GMT
ENV OTP_VERSION=24.0.2 REBAR3_VERSION=3.16.1
# Wed, 23 Jun 2021 19:11:13 GMT
LABEL org.opencontainers.image.version=24.0.2
# Wed, 23 Jun 2021 19:25:22 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4abca2cda7fc962ad65575e5ed834dd69c745e7e637f92cfd49f384a281d0f18" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 23 Jun 2021 19:25:37 GMT
CMD ["erl"]
# Wed, 23 Jun 2021 19:25:44 GMT
ENV REBAR_VERSION=2.6.4
# Wed, 23 Jun 2021 19:26:05 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Wed, 23 Jun 2021 19:26:51 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="a14711b09f6e1fc1b080b79d78c304afebcbb7fafed9d0972eb739f0ed89121b" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
```

-	Layers:
	-	`sha256:83f72610ec8bc58c0c3a70f0bdf9d866e8d0156845a9aa24bc0ed2fdaf0fd8b4`  
		Last Modified: Wed, 23 Jun 2021 00:36:35 GMT  
		Size: 54.2 MB (54182463 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3cdd4a29fac3f4917f56dc5f262d8365826de2b3fb72d6188dc15aa46e8e6d6`  
		Last Modified: Wed, 23 Jun 2021 03:13:08 GMT  
		Size: 8.3 MB (8271984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de85832cf44484bc526bc3e5af3698f3f1b7e753c47e9be91655ca62e7d3abd3`  
		Last Modified: Wed, 23 Jun 2021 03:13:09 GMT  
		Size: 10.7 MB (10727812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8657fc4cb7f4239ffd0cc0698de0121b50102bdc97b4c558bf496726505f2962`  
		Last Modified: Wed, 23 Jun 2021 03:13:34 GMT  
		Size: 57.5 MB (57457627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ca33ad4a459e29bc590b75491f2f686e995e93aa77e8fdcf0db365947461807`  
		Last Modified: Wed, 23 Jun 2021 03:14:21 GMT  
		Size: 203.3 MB (203281849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3339cd3e88a51509ba6030f6f343bdddfc827d92461eb010247bef7c19a5925`  
		Last Modified: Wed, 23 Jun 2021 20:13:45 GMT  
		Size: 167.5 MB (167511219 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9a017b873c0a2a455a1456ba7cbfba3b9263b2a3757eba8da56abf7f7752d59`  
		Last Modified: Wed, 23 Jun 2021 20:13:12 GMT  
		Size: 196.5 KB (196541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3ef5c976b26542e071b6b30ba564bc1a6e50ac20b18ebe06ab8ec54befcfc10d`  
		Last Modified: Wed, 23 Jun 2021 20:13:14 GMT  
		Size: 955.9 KB (955853 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:latest` - linux; s390x

```console
$ docker pull erlang@sha256:7ff026259341170a1a6af58dd74fbcd33565b396c3dfbb157c6e0db2c55a53fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **456.4 MB (456449741 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d22c390325ac86f612d8608f7e1922150102204a630324c9955975c999dedca4`
-	Default Command: `["erl"]`

```dockerfile
# Tue, 22 Jun 2021 23:42:13 GMT
ADD file:b935574081a3fbceb534880a35e5245e10c52a3b9d70224811e221b4c6254cfe in / 
# Tue, 22 Jun 2021 23:42:16 GMT
CMD ["bash"]
# Wed, 23 Jun 2021 00:05:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:06:04 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 23 Jun 2021 00:06:26 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:07:22 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:14:24 GMT
ENV OTP_VERSION=24.0.2 REBAR3_VERSION=3.16.1
# Wed, 23 Jun 2021 00:14:25 GMT
LABEL org.opencontainers.image.version=24.0.2
# Wed, 23 Jun 2021 00:22:06 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4abca2cda7fc962ad65575e5ed834dd69c745e7e637f92cfd49f384a281d0f18" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make -j$(nproc) docs DOC_TARGETS=chunks 	  && make install install-docs DOC_TARGETS=chunks ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 23 Jun 2021 00:22:13 GMT
CMD ["erl"]
# Wed, 23 Jun 2021 00:22:13 GMT
ENV REBAR_VERSION=2.6.4
# Wed, 23 Jun 2021 00:22:17 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Wed, 23 Jun 2021 00:22:36 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="a14711b09f6e1fc1b080b79d78c304afebcbb7fafed9d0972eb739f0ed89121b" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
```

-	Layers:
	-	`sha256:2b8d113de06cefaa0768df3e10da0c3b8272e15922e18ea75b0bb4dee23b551d`  
		Last Modified: Tue, 22 Jun 2021 23:45:28 GMT  
		Size: 49.0 MB (49003924 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1de1b6d51a91a64482d6eabf778b8c4e433f7dc198440476d01d0dbb31aee4fe`  
		Last Modified: Wed, 23 Jun 2021 00:12:08 GMT  
		Size: 7.4 MB (7400480 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d64019084b252c52592ff8cab3bf20be9bab2801ea36e88025071f901f1cb38e`  
		Last Modified: Wed, 23 Jun 2021 00:12:08 GMT  
		Size: 9.9 MB (9882902 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:481cb3d9acd652b3fd56e606ff28a1bb48aa89be3365577a33d2cd35c908d867`  
		Last Modified: Wed, 23 Jun 2021 00:12:24 GMT  
		Size: 51.4 MB (51380256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1743770944cccb82c795de20a9395efe75855871d9d8f58a7e3bf8eaef915cd7`  
		Last Modified: Wed, 23 Jun 2021 00:12:52 GMT  
		Size: 176.9 MB (176880014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:199cb9f671aa599f20824be00fc28c9ab9ceca6164058b6cf28aba481664ace5`  
		Last Modified: Wed, 23 Jun 2021 01:05:52 GMT  
		Size: 160.7 MB (160749808 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac3746e330c892c2832c1a37df0d626c662441f0e40f99e8dd3586b2734abec0`  
		Last Modified: Wed, 23 Jun 2021 01:05:33 GMT  
		Size: 196.5 KB (196496 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc6ce902ee058adaebf79f62aca05a7b5a07e33e81d7f1b3088491e62ef8caf`  
		Last Modified: Wed, 23 Jun 2021 01:05:33 GMT  
		Size: 955.9 KB (955861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
