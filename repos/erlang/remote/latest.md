## `erlang:latest`

```console
$ docker pull erlang@sha256:4500df4fb4908a5478c3e29dae5fa86ce828ff041f655eb7b196f99534ef79a2
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
$ docker pull erlang@sha256:8547c5a156aa6104d9688cf3c1211731423a33a23a548ee7ecda8a5bb1a319a8
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **471.4 MB (471387468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a8c6afe9eb8ef654136d7c5dc0ba5e121fde87b53e9748d7b7986ab8c477ba0`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 01 Feb 2020 17:20:38 GMT
ADD file:a5ec219cbfc4e0c31e7df48cc51abd9a5b92754e15403b2ab726e25042041680 in / 
# Sat, 01 Feb 2020 17:20:39 GMT
CMD ["bash"]
# Sun, 02 Feb 2020 00:18:59 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:19:06 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sun, 02 Feb 2020 00:19:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sun, 02 Feb 2020 00:20:18 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Feb 2020 00:20:07 GMT
ENV OTP_VERSION=22.2.6 REBAR3_VERSION=3.13.0
# Fri, 07 Feb 2020 00:20:08 GMT
LABEL org.opencontainers.image.version=22.2.6
# Fri, 07 Feb 2020 00:45:53 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4cf44ed12f657c309a2c00e7806f36f56a88e5b74de6814058796561f3842f66" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 07 Feb 2020 00:45:54 GMT
CMD ["erl"]
# Fri, 07 Feb 2020 00:45:55 GMT
ENV REBAR_VERSION=2.6.4
# Fri, 07 Feb 2020 00:46:03 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Fri, 07 Feb 2020 00:47:00 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="49ecf89d04676d077712a10d8252bbda73998a3badf8b342481530fbc685a123" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
```

-	Layers:
	-	`sha256:dc65f448a2e2f2ea557e69ed9ac65aa8ac0e16f1bce68f90de910b4d5a2f1ba1`  
		Last Modified: Sat, 01 Feb 2020 17:26:04 GMT  
		Size: 50.4 MB (50379770 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:346ffb2b67d7b35729673ced818325ed0ea57284e69de67f8bbc48c2bf294716`  
		Last Modified: Sun, 02 Feb 2020 00:37:48 GMT  
		Size: 7.8 MB (7811673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dea4ecac934f71d68d4f5edb171f6cff42588edfa3f70ba8709be56e321eeddc`  
		Last Modified: Sun, 02 Feb 2020 00:37:49 GMT  
		Size: 10.0 MB (9996251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac92ddf84b35dac36ef6632f8d5a0c9c2d7038f6018f2d4fa1be056d90bd366`  
		Last Modified: Sun, 02 Feb 2020 00:38:05 GMT  
		Size: 51.8 MB (51791113 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3ca60abc08a00e84d4fb6bd20998f38c2e171f6e085e5e7c26908be7223ea7c`  
		Last Modified: Sun, 02 Feb 2020 00:38:57 GMT  
		Size: 192.2 MB (192169044 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3817d5f4180e6b394cd48881f4737fce63f3fab6f6deb55ecd88425eab071cfb`  
		Last Modified: Fri, 07 Feb 2020 01:37:37 GMT  
		Size: 158.2 MB (158230682 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4449e4102310bf958b7408424f5d4ada6cd72e5348abc5e42e3945f14f317a`  
		Last Modified: Fri, 07 Feb 2020 01:35:50 GMT  
		Size: 197.0 KB (196963 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7baead623b008645085db4fbcd9708f6ce91d51c5c1780694a259565ce53dd6`  
		Last Modified: Fri, 07 Feb 2020 01:35:51 GMT  
		Size: 812.0 KB (811972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:latest` - linux; arm variant v7

```console
$ docker pull erlang@sha256:93e2598f5f3053bc1865db11187d4da55ac4f8b13766586a41f4bff147948c1f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **424.3 MB (424330272 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:409ab7ef318ce100ad2bfb06d202acb1e43af97347b2533bda8218b9fe813361`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 01 Feb 2020 17:00:06 GMT
ADD file:a57a312731f174c4b03031908ff95f49d7055d8c196439f0ed07ed9c4834d993 in / 
# Sat, 01 Feb 2020 17:00:08 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:00:08 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:00:24 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:01:04 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:03:27 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Feb 2020 00:49:14 GMT
ENV OTP_VERSION=22.2.6 REBAR3_VERSION=3.13.0
# Fri, 07 Feb 2020 00:49:15 GMT
LABEL org.opencontainers.image.version=22.2.6
# Fri, 07 Feb 2020 00:57:40 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4cf44ed12f657c309a2c00e7806f36f56a88e5b74de6814058796561f3842f66" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 07 Feb 2020 00:57:46 GMT
CMD ["erl"]
# Fri, 07 Feb 2020 00:57:47 GMT
ENV REBAR_VERSION=2.6.4
# Fri, 07 Feb 2020 00:57:55 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Fri, 07 Feb 2020 00:58:40 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="49ecf89d04676d077712a10d8252bbda73998a3badf8b342481530fbc685a123" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
```

-	Layers:
	-	`sha256:9bbb41bca8c6254da5088d03354297b1309dc75c2ccc738416025f89709ae5ee`  
		Last Modified: Sat, 01 Feb 2020 17:07:28 GMT  
		Size: 45.9 MB (45859700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:239e4acdbc2ab88c89aa359fbab11429ea6d7bd93ea589a22c6bbb833ff82b93`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 7.1 MB (7096223 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83d6b4707a3c3aff9cb939fc058b869c5412e78c37e43eb0b653565460495537`  
		Last Modified: Sat, 01 Feb 2020 18:25:50 GMT  
		Size: 9.3 MB (9343278 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e096c4fc8c629edca6da3ce5a9e95288512cb11e3d3d01a6e49078d19c2acca`  
		Last Modified: Sat, 01 Feb 2020 18:26:13 GMT  
		Size: 47.3 MB (47315591 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6953ecf4273071529462518748f048f49a05530ae24d8fc6841919de312f2fc`  
		Last Modified: Sat, 01 Feb 2020 18:27:03 GMT  
		Size: 168.4 MB (168379144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d498e4eca7d7b17241fca5d91476af0750910f9e4000f5d7e2f8871bbebf810`  
		Last Modified: Fri, 07 Feb 2020 01:14:37 GMT  
		Size: 145.3 MB (145327404 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc743fde29aa59eaca124776d6a89eda25ae8449a469c17ed115de52e82a38d2`  
		Last Modified: Fri, 07 Feb 2020 01:12:39 GMT  
		Size: 197.0 KB (196959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:514c3054f5daca93fc36ae619478d35c02afb911689b369b605cd51abe2c056f`  
		Last Modified: Fri, 07 Feb 2020 01:12:40 GMT  
		Size: 812.0 KB (811973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:latest` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:abb3e730708ec2877031b54bc079a3188f43801cc3076c8452a68803196c8e0f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **454.5 MB (454523404 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57e00a0dc76b7d1e9fed210b1191e1683129d96727711964791911e8802ece9f`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 01 Feb 2020 16:40:50 GMT
ADD file:b423f4b0ed41dfe1334031fe9b21f7e1c88ccb031d7e8f2ff165d618323424d7 in / 
# Sat, 01 Feb 2020 16:40:53 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:18:39 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:18:51 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:19:27 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:21:41 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Feb 2020 00:44:38 GMT
ENV OTP_VERSION=22.2.6 REBAR3_VERSION=3.13.0
# Fri, 07 Feb 2020 00:44:38 GMT
LABEL org.opencontainers.image.version=22.2.6
# Fri, 07 Feb 2020 00:52:42 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4cf44ed12f657c309a2c00e7806f36f56a88e5b74de6814058796561f3842f66" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 07 Feb 2020 00:52:49 GMT
CMD ["erl"]
# Fri, 07 Feb 2020 00:52:51 GMT
ENV REBAR_VERSION=2.6.4
# Fri, 07 Feb 2020 00:53:08 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Fri, 07 Feb 2020 00:53:52 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="49ecf89d04676d077712a10d8252bbda73998a3badf8b342481530fbc685a123" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
```

-	Layers:
	-	`sha256:bc03a7ced18fc43ea9523dfb256d2c3fbb835dc0bb54bdb7fd309edf936a87e7`  
		Last Modified: Sat, 01 Feb 2020 16:46:06 GMT  
		Size: 49.2 MB (49171687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cba9d528c1473d79c18b401d44ca06b9733d9c51a8699b98e8325c9de60b9739`  
		Last Modified: Sat, 01 Feb 2020 17:34:59 GMT  
		Size: 7.7 MB (7680993 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:981400d5d268dc989681d5f308b7d2e381809f0bcc82429f443f7539cf6117ba`  
		Last Modified: Sat, 01 Feb 2020 17:34:59 GMT  
		Size: 10.0 MB (9983754 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0b2d547b8bc79a444406e56d724fb7d961c953e7f2797de4f55b29abee5605f`  
		Last Modified: Sat, 01 Feb 2020 17:35:22 GMT  
		Size: 52.1 MB (52102938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb5086353cdd3bb763311aa0618b7867d51f7fe7393d00e0643b1618588d36a9`  
		Last Modified: Sat, 01 Feb 2020 17:36:12 GMT  
		Size: 183.7 MB (183697606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc33579f5fcf4d9174c836b4f78d57c2261f796166e0cea6e87c2ea3e6395ce7`  
		Last Modified: Fri, 07 Feb 2020 01:08:41 GMT  
		Size: 150.9 MB (150877486 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16373e50a51f5f0dfe6b6b1aed480a8171d6d8fc49d6486a374d479c55633af6`  
		Last Modified: Fri, 07 Feb 2020 01:08:04 GMT  
		Size: 197.0 KB (196969 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf33a2f7683cd08a1329936e1820cc857595bc28241319254284e679e0c4cac1`  
		Last Modified: Fri, 07 Feb 2020 01:08:05 GMT  
		Size: 812.0 KB (811971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:latest` - linux; 386

```console
$ docker pull erlang@sha256:7b4dd216737d746e6f469440abf2610d12bb8febfd88f821740e19f97d7a5de3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **481.7 MB (481739465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b53f599b7a916ae892019c24ad33e138ec43b0eacebaedac2db2e50e889866a`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 01 Feb 2020 16:39:21 GMT
ADD file:b637f96d557a570f8ab83b28f7b9cdd128958359dd30dc2e03df70b799e132aa in / 
# Sat, 01 Feb 2020 16:39:21 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:23:48 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:24:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:24:25 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:25:45 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Feb 2020 00:39:09 GMT
ENV OTP_VERSION=22.2.5 REBAR3_VERSION=3.13.0
# Wed, 05 Feb 2020 00:39:09 GMT
LABEL org.opencontainers.image.version=22.2.5
# Wed, 05 Feb 2020 01:03:57 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="a2359af240c7f629a4f9f19a9c0ba94e6ba024ed9fc4728c8ae55ea7c8c0e260" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 05 Feb 2020 01:03:58 GMT
CMD ["erl"]
# Wed, 05 Feb 2020 01:03:58 GMT
ENV REBAR_VERSION=2.6.4
# Wed, 05 Feb 2020 01:04:04 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Wed, 05 Feb 2020 01:05:01 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="49ecf89d04676d077712a10d8252bbda73998a3badf8b342481530fbc685a123" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
```

-	Layers:
	-	`sha256:2b34644a479c82db66a603c0b0a1d990911345f8646498fa9b050f306d0e6bf2`  
		Last Modified: Sat, 01 Feb 2020 16:44:10 GMT  
		Size: 51.1 MB (51141949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c2f611c9392c4fe86735b477d61fda0e95ea77486175a737114c51586ecce86`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 8.0 MB (7981506 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69713757cc2d87c3255331d40f5061a73ef412208961f1ddd67a59a375397fda`  
		Last Modified: Sat, 01 Feb 2020 17:42:17 GMT  
		Size: 10.3 MB (10338479 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:956cf07a321afcfed99809a380a1905660e378188fd33d97f136551450be347a`  
		Last Modified: Sat, 01 Feb 2020 17:42:36 GMT  
		Size: 53.4 MB (53380753 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c8bfbd246f3a4ba9d861315c676a9a9e6524857c085e71b18b492882b063bff`  
		Last Modified: Sat, 01 Feb 2020 17:43:24 GMT  
		Size: 198.7 MB (198719863 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:553a65a22ddfb62bee254eb6abf49b8dd58f38bd93a1d8a325cc49fa22a4b538`  
		Last Modified: Wed, 05 Feb 2020 02:44:03 GMT  
		Size: 159.2 MB (159167960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ebebd89e79cd8ebdafb9426d6865e1c4446699fec9e9c96a73f2149dffc9a18`  
		Last Modified: Wed, 05 Feb 2020 02:43:12 GMT  
		Size: 196.9 KB (196932 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a76b7b23c050025e5a37140220181078c8eb73a05f6563b7556a6a86f3aa4a`  
		Last Modified: Wed, 05 Feb 2020 02:43:11 GMT  
		Size: 812.0 KB (812023 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:latest` - linux; ppc64le

```console
$ docker pull erlang@sha256:4bc9de6efc5d37e289454ec7cb544c6977eedd4968ddc64527cd7502f8b7b211
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **493.5 MB (493513598 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39a79ddf925f948f6aa4fe8e550d10d2f286bf24b9016fbe540a98cbab306f1e`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 01 Feb 2020 17:17:37 GMT
ADD file:8e8c5417abc372541fe34cddec6fe8625ded93da51d1f5488e0aece309a3fd25 in / 
# Sat, 01 Feb 2020 17:17:45 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 18:37:43 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:38:16 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 18:39:29 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 18:45:55 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Feb 2020 01:24:27 GMT
ENV OTP_VERSION=22.2.6 REBAR3_VERSION=3.13.0
# Fri, 07 Feb 2020 01:24:32 GMT
LABEL org.opencontainers.image.version=22.2.6
# Fri, 07 Feb 2020 01:35:33 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4cf44ed12f657c309a2c00e7806f36f56a88e5b74de6814058796561f3842f66" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 07 Feb 2020 01:35:46 GMT
CMD ["erl"]
# Fri, 07 Feb 2020 01:35:53 GMT
ENV REBAR_VERSION=2.6.4
# Fri, 07 Feb 2020 01:36:08 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Fri, 07 Feb 2020 01:36:52 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="49ecf89d04676d077712a10d8252bbda73998a3badf8b342481530fbc685a123" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
```

-	Layers:
	-	`sha256:a2d5a5ee40c1df8706e6db684b090e0e4297581ff38256a81222ea8be61180fc`  
		Last Modified: Sat, 01 Feb 2020 17:25:27 GMT  
		Size: 54.1 MB (54132833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7f35d9825c38e7e0c3f571e8abe513b3b11599bd64a853ace5494e8c1ebe12a`  
		Last Modified: Sat, 01 Feb 2020 19:17:26 GMT  
		Size: 8.3 MB (8252196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27e6d793f7577bc28e3d8da62385244985a340fe31c9eaa920a54185f9d46eb8`  
		Last Modified: Sat, 01 Feb 2020 19:17:26 GMT  
		Size: 10.7 MB (10727116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa97a0399500f41c90805413f9dd183cb0036f1446b766e62ad6310e2357d9b8`  
		Last Modified: Sat, 01 Feb 2020 19:18:21 GMT  
		Size: 57.4 MB (57392303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e66b06b3e1c485a1d01f726e2dedb4ebb96a236053344697e5d27170fa2c818c`  
		Last Modified: Sat, 01 Feb 2020 19:19:59 GMT  
		Size: 203.0 MB (202991708 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380cb297910aa815bf4fc43f9056c4656e142c72132462ce84aef3e2098f62ef`  
		Last Modified: Fri, 07 Feb 2020 01:58:39 GMT  
		Size: 159.0 MB (159008498 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c21a99db838fc7c4916649f380248b4d46086a507ec01226825a44d79241d4d`  
		Last Modified: Fri, 07 Feb 2020 01:56:51 GMT  
		Size: 197.0 KB (196971 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:304d9e134bc49f5708a6ae0cc5f7727200b8795d5eae552793dcbea997d7f623`  
		Last Modified: Fri, 07 Feb 2020 01:56:52 GMT  
		Size: 812.0 KB (811973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:latest` - linux; s390x

```console
$ docker pull erlang@sha256:0b8582eba38cd30adee66f7d0f24115f11c130e791f3ac5639cc8a2b3cde095c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **447.4 MB (447372700 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ac8f3465490bb1bca6ea35cf40c374a7a4aed025a5509195325c4f6e12647fb8`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 01 Feb 2020 16:42:14 GMT
ADD file:642aef2e391d18e3999374d6068f29ccc5ad62b25a0d18c852a6b5534daa18f7 in / 
# Sat, 01 Feb 2020 16:42:17 GMT
CMD ["bash"]
# Sat, 01 Feb 2020 17:50:06 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:50:10 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Sat, 01 Feb 2020 17:50:31 GMT
RUN apt-get update && apt-get install -y --no-install-recommends 		git 		mercurial 		openssh-client 		subversion 				procps 	&& rm -rf /var/lib/apt/lists/*
# Sat, 01 Feb 2020 17:51:37 GMT
RUN set -ex; 	apt-get update; 	apt-get install -y --no-install-recommends 		autoconf 		automake 		bzip2 		dpkg-dev 		file 		g++ 		gcc 		imagemagick 		libbz2-dev 		libc6-dev 		libcurl4-openssl-dev 		libdb-dev 		libevent-dev 		libffi-dev 		libgdbm-dev 		libglib2.0-dev 		libgmp-dev 		libjpeg-dev 		libkrb5-dev 		liblzma-dev 		libmagickcore-dev 		libmagickwand-dev 		libmaxminddb-dev 		libncurses5-dev 		libncursesw5-dev 		libpng-dev 		libpq-dev 		libreadline-dev 		libsqlite3-dev 		libssl-dev 		libtool 		libwebp-dev 		libxml2-dev 		libxslt-dev 		libyaml-dev 		make 		patch 		unzip 		xz-utils 		zlib1g-dev 				$( 			if apt-cache show 'default-libmysqlclient-dev' 2>/dev/null | grep -q '^Version:'; then 				echo 'default-libmysqlclient-dev'; 			else 				echo 'libmysqlclient-dev'; 			fi 		) 	; 	rm -rf /var/lib/apt/lists/*
# Fri, 07 Feb 2020 01:01:21 GMT
ENV OTP_VERSION=22.2.6 REBAR3_VERSION=3.13.0
# Fri, 07 Feb 2020 01:01:21 GMT
LABEL org.opencontainers.image.version=22.2.6
# Fri, 07 Feb 2020 01:06:42 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="4cf44ed12f657c309a2c00e7806f36f56a88e5b74de6814058796561f3842f66" 	&& runtimeDeps='libodbc1 			libsctp1 			libwxgtk3.0' 	&& buildDeps='unixodbc-dev 			libsctp-dev 			libwxgtk3.0-dev' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Fri, 07 Feb 2020 01:06:49 GMT
CMD ["erl"]
# Fri, 07 Feb 2020 01:06:49 GMT
ENV REBAR_VERSION=2.6.4
# Fri, 07 Feb 2020 01:06:52 GMT
RUN set -xe 	&& REBAR_DOWNLOAD_URL="https://github.com/rebar/rebar/archive/${REBAR_VERSION}.tar.gz" 	&& REBAR_DOWNLOAD_SHA256="577246bafa2eb2b2c3f1d0c157408650446884555bf87901508ce71d5cc0bd07" 	&& mkdir -p /usr/src/rebar-src 	&& curl -fSL -o rebar-src.tar.gz "$REBAR_DOWNLOAD_URL" 	&& echo "$REBAR_DOWNLOAD_SHA256 rebar-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar-src.tar.gz -C /usr/src/rebar-src --strip-components=1 	&& rm rebar-src.tar.gz 	&& cd /usr/src/rebar-src 	&& ./bootstrap 	&& install -v ./rebar /usr/local/bin/ 	&& rm -rf /usr/src/rebar-src
# Fri, 07 Feb 2020 01:07:15 GMT
RUN set -xe 	&& REBAR3_DOWNLOAD_URL="https://github.com/erlang/rebar3/archive/${REBAR3_VERSION}.tar.gz" 	&& REBAR3_DOWNLOAD_SHA256="49ecf89d04676d077712a10d8252bbda73998a3badf8b342481530fbc685a123" 	&& mkdir -p /usr/src/rebar3-src 	&& curl -fSL -o rebar3-src.tar.gz "$REBAR3_DOWNLOAD_URL" 	&& echo "$REBAR3_DOWNLOAD_SHA256 rebar3-src.tar.gz" | sha256sum -c - 	&& tar -xzf rebar3-src.tar.gz -C /usr/src/rebar3-src --strip-components=1 	&& rm rebar3-src.tar.gz 	&& cd /usr/src/rebar3-src 	&& HOME=$PWD ./bootstrap 	&& install -v ./rebar3 /usr/local/bin/ 	&& rm -rf /usr/src/rebar3-src
```

-	Layers:
	-	`sha256:6f3b736b312bfd59fd7947524542ae1d57ed4564aefaafdf0ccfb7d600f7978f`  
		Last Modified: Sat, 01 Feb 2020 16:45:36 GMT  
		Size: 49.0 MB (48954499 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6eca02855c81b470d73964fc93a8a5e484c5ce5dd6782210cc15b8aca2d28684`  
		Last Modified: Sat, 01 Feb 2020 18:03:52 GMT  
		Size: 7.4 MB (7381759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88ecd1a9e0aa67e009dc11b696d0a2029c3bb506e5058e13434114e16ad7a290`  
		Last Modified: Sat, 01 Feb 2020 18:03:53 GMT  
		Size: 9.9 MB (9882030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:114b7e56002fcad21b16ab9d3774a372824925547f59e9580bc61ec3cee41394`  
		Last Modified: Sat, 01 Feb 2020 18:04:07 GMT  
		Size: 51.3 MB (51326330 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84a628df1a6847d135507263b6987b1bc583d7bfdd30772ae3f7fb008f2bca33`  
		Last Modified: Sat, 01 Feb 2020 18:04:43 GMT  
		Size: 176.7 MB (176722026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fada8a82616851b632f57f89b82f99445ba9226c45ce1d730d42c32d77cc789d`  
		Last Modified: Fri, 07 Feb 2020 01:20:54 GMT  
		Size: 152.1 MB (152097118 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c9b6e4078e793e437d3dd0ad714c2ea2a7bcda801895858ef9dadb7ee30a8b1`  
		Last Modified: Fri, 07 Feb 2020 01:18:48 GMT  
		Size: 197.0 KB (196966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9240b5133ec240204e2d4b2a75a8962544e6650f0a2b086b1bb8ea9cabf706c9`  
		Last Modified: Fri, 07 Feb 2020 01:18:17 GMT  
		Size: 812.0 KB (811972 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
