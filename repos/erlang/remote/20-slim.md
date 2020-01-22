## `erlang:20-slim`

```console
$ docker pull erlang@sha256:9c81e467fd302367286b5622929609cf7ed48a5f493be8ef7375bc5dffd5d904
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `erlang:20-slim` - linux; amd64

```console
$ docker pull erlang@sha256:b4f91699ec9a279f3e58726c663dc81ff627e1f3cfa95a4216e67b5c8007dff5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **110.6 MB (110645704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:57bdae840f4ae959074c8a20d066f3b2a959179dc9f79cc6377f53e6bf40040d`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:23:33 GMT
ADD file:8f7dc710e276f54a3a73d34b6b8fa261950a781d68ceb7401fa18dabc601c5a5 in / 
# Sat, 28 Dec 2019 04:23:34 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 11:21:37 GMT
ENV OTP_VERSION=20.3.8.24
# Sat, 28 Dec 2019 11:39:16 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="588e34a89f9ea8ebc3bda0918e4e1f4f7366888278f5e7ece60f6f1fa42aef60" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Sat, 28 Dec 2019 11:39:16 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:146bd6a886182fde06fbf747470b1c89814bc8ab1c96fdf1aef6107171959fe6`  
		Last Modified: Sat, 28 Dec 2019 04:28:25 GMT  
		Size: 45.4 MB (45380744 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a0581f391eb0382f37a09cb1eba5544a83bbef6980363d28f7c2634eb091ba8`  
		Last Modified: Sat, 28 Dec 2019 12:56:17 GMT  
		Size: 65.3 MB (65264960 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:20-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:ed0adcd5db52c98e8c99f6d194f53667bf3a22441f28c9c5684932a1086579f3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **102.3 MB (102347986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f25163c3d79c9c0045b2a1715af71cea35d3836c5c3f47a7f9987eb70f494c86`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:19 GMT
ADD file:5692a55e4805d33baa21e559cc0bb86fb91422171345ddd332fa5514285a3401 in / 
# Sat, 28 Dec 2019 05:03:25 GMT
CMD ["bash"]
# Wed, 22 Jan 2020 01:56:35 GMT
ENV OTP_VERSION=20.3.8.25
# Wed, 22 Jan 2020 02:03:38 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="36f36753b8cf4db35f0d0c1cb88a32d4309670859174492ff8d10f5cf1f93720" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 22 Jan 2020 02:03:41 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:b531ae4a39253d883a11291e842b7e1aa9dae38f9d9b77ddea55b2625ce986e3`  
		Last Modified: Sat, 28 Dec 2019 05:10:53 GMT  
		Size: 42.1 MB (42108124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:959772c687b635e3661a1f1107a3508adce7040a69c0a31afe0843b042e743a0`  
		Last Modified: Wed, 22 Jan 2020 02:15:58 GMT  
		Size: 60.2 MB (60239862 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:20-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:99c6e9ba5572a80effa7354c38b7b204d46acba2bacd29c17df0041747fd6cd9
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **104.6 MB (104591896 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ce8b5380485c950e8897832e629a38bf14130baedbd7ae26871add2bfd3d88ea`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:15 GMT
ADD file:e439b3c387852978811a6a5a058745ebb9392da7e8936beb4f37ff076e656213 in / 
# Sat, 28 Dec 2019 04:43:17 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:14:14 GMT
ENV OTP_VERSION=20.3.8.24
# Sat, 28 Dec 2019 07:21:35 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="588e34a89f9ea8ebc3bda0918e4e1f4f7366888278f5e7ece60f6f1fa42aef60" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:21:38 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:d07bcf5901dfa793fa6b2c4c617e86bcef315b0b092cbfd1a929eefedaf8e3f2`  
		Last Modified: Sat, 28 Dec 2019 04:48:57 GMT  
		Size: 43.2 MB (43166476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76860b6fd222b75b225e260edbe9df6c00eb9ef7881aa447394ad1280224e91f`  
		Last Modified: Sat, 28 Dec 2019 08:11:02 GMT  
		Size: 61.4 MB (61425420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:20-slim` - linux; 386

```console
$ docker pull erlang@sha256:c5b3c9327e325268de74058bff13f80570c61ba5ac00949b276a4b1b14218a96
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **114.4 MB (114445688 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab5552798c46df226c17120b1cf943494fe5807397b57b0e57fab6683a480f9f`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:51 GMT
ADD file:f348ed8c5f7efee9f7e88d9a9bd1d57bca1bf445d486996cb6168da85c0bd43b in / 
# Sat, 28 Dec 2019 04:41:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:24:59 GMT
ENV OTP_VERSION=20.3.8.24
# Sat, 28 Dec 2019 07:42:31 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="588e34a89f9ea8ebc3bda0918e4e1f4f7366888278f5e7ece60f6f1fa42aef60" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:42:32 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:410821d7ff8b427b8dfb93dcf31b1836a617f5c09be71f83a16ef2c5946ee700`  
		Last Modified: Sat, 28 Dec 2019 04:47:20 GMT  
		Size: 46.1 MB (46100094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:111c385e17384109ad6e7f56003da7aec536657149ff13f01cbb658e693389fc`  
		Last Modified: Sat, 28 Dec 2019 08:46:32 GMT  
		Size: 68.3 MB (68345594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:20-slim` - linux; ppc64le

```console
$ docker pull erlang@sha256:c54720ef5947e563cc44a309699c3734ac87f1f048265842819016fddbc03669
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **108.0 MB (107977500 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6c03ccc32a60531d18ddf6471ad40c7877c622efd2ec75c5ee0f93cdbc9a63f1`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:22:59 GMT
ADD file:0da9c5c67cad579be1a33f0f66df515de7f3ad992050c39cbaac281a01be41b3 in / 
# Sat, 28 Dec 2019 04:23:02 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:27:06 GMT
ENV OTP_VERSION=20.3.8.24
# Sat, 28 Dec 2019 08:36:04 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="588e34a89f9ea8ebc3bda0918e4e1f4f7366888278f5e7ece60f6f1fa42aef60" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:36:08 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:32185d9fc6268c6a6d87060ea324482fa22129c0f06d0f35e1376ca27b5399a0`  
		Last Modified: Sat, 28 Dec 2019 04:32:44 GMT  
		Size: 45.7 MB (45652475 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce1d72304673235037aa0cce03a2e53ae80932bf4d47b2561070fc8940156c6b`  
		Last Modified: Sat, 28 Dec 2019 08:41:05 GMT  
		Size: 62.3 MB (62325025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:20-slim` - linux; s390x

```console
$ docker pull erlang@sha256:94806bc9b5f5c9aa19d2b77d9f9a317bb31ccc79a394a1d65fab4a326f4af362
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **109.1 MB (109148869 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:41d9f04b1f1099b1f9e2a9b5e6436b3ae478eb5dbd2bfacd0e56877f4d7e805d`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:08 GMT
ADD file:b85ece7344f0ad0749b115e76a51a3b9f322e23bcc8c692cd2edff403ba8840e in / 
# Sat, 28 Dec 2019 04:43:08 GMT
CMD ["bash"]
# Wed, 22 Jan 2020 02:15:50 GMT
ENV OTP_VERSION=20.3.8.25
# Wed, 22 Jan 2020 02:19:42 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="36f36753b8cf4db35f0d0c1cb88a32d4309670859174492ff8d10f5cf1f93720" 	&& fetchDeps=' 		curl 		ca-certificates' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $fetchDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256  otp-src.tar.gz" | sha256sum -c - 	&& runtimeDeps=' 		libodbc1 		libssl1.1 		libsctp1 	' 	&& buildDeps=' 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl-dev 		libsctp-dev 	' 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& export ERL_TOP="/usr/src/otp_src_${OTP_VERSION%%@*}" 	&& mkdir -vp $ERL_TOP 	&& tar -xzf otp-src.tar.gz -C $ERL_TOP --strip-components=1 	&& rm otp-src.tar.gz 	&& ( cd $ERL_TOP 	  && ./otp_build autoconf 	  && gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	  && ./configure --build="$gnuArch" 	  && make -j$(nproc) 	  && make install ) 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps $fetchDeps 	&& rm -rf $ERL_TOP /var/lib/apt/lists/*
# Wed, 22 Jan 2020 02:19:42 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:5bf261872a9b22035011c2bf77259c73389d0d5786e4b43bee1df89b5dfada2f`  
		Last Modified: Sat, 28 Dec 2019 04:46:24 GMT  
		Size: 45.2 MB (45241644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f99f023315b9f700b450e6a59a4e74f1bc627f464699838c0a4229d014cae5af`  
		Last Modified: Wed, 22 Jan 2020 02:27:13 GMT  
		Size: 63.9 MB (63907225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
