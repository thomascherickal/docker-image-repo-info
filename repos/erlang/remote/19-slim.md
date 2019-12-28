## `erlang:19-slim`

```console
$ docker pull erlang@sha256:9315ab11aa2de660b6b2dadd5bedcb73639e39ff11c2252274b987c885e0b229
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; s390x

### `erlang:19-slim` - linux; amd64

```console
$ docker pull erlang@sha256:5a3256735e418a63dddc58c16b623e84ddb61f33eff46dc5743e53272178bc53
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **257.8 MB (257793344 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8bfcb589a0fa50fdd71783f1ebf2183993bcad64fe44a0f5e00400af4f59354`
-	Default Command: `["erl"]`

```dockerfile
# Fri, 22 Nov 2019 14:58:56 GMT
ADD file:152359c10cf61d80091bfd19e7e1968a538bebebfa048dca0386e35e1e999730 in / 
# Fri, 22 Nov 2019 14:58:56 GMT
CMD ["bash"]
# Sat, 23 Nov 2019 04:13:29 GMT
ENV OTP_VERSION=19.3.6.13
# Sat, 23 Nov 2019 04:35:48 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="11a914176a33068226644f4e999ecc6e965ab1c60a324d90020f164641631fae" 	&& runtimeDeps=' 		libodbc1 		libssl1.0.2 		libsctp1 		libwxgtk3.0 	' 	&& buildDeps=' 		curl 		ca-certificates 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl1.0-dev 		libsctp-dev 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256 otp-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/otp-src 	&& tar -xzf otp-src.tar.gz -C /usr/src/otp-src --strip-components=1 	&& rm otp-src.tar.gz 	&& cd /usr/src/otp-src 	&& ./otp_build autoconf 	&& gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	&& ./configure --build="$gnuArch" 		--enable-dirty-schedulers 	&& make -j$(nproc) 	&& make install 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/otp-src /var/lib/apt/lists/*
# Sat, 23 Nov 2019 04:35:49 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:844c33c7e6ea19e3f6847e0667befdfb3ef02d6fc735b22c2d070261b6263b97`  
		Last Modified: Fri, 22 Nov 2019 15:06:19 GMT  
		Size: 45.4 MB (45380759 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9951f9b66494e1dbaeb95a721f63fe7818ad2e1b1d48f196a87c988cb4b1d875`  
		Last Modified: Sat, 23 Nov 2019 05:08:48 GMT  
		Size: 212.4 MB (212412585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:19-slim` - linux; arm variant v7

```console
$ docker pull erlang@sha256:ddf5e660efca99c1dbe903a9250f4a2da131fd15ec5b9eba92b4f155a00c1502
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **242.8 MB (242842532 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f3c1057ef0f7164329a2de2b80d09a265a0cb5fdac71e75f18a0b3cf4f5185b6`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 05:03:19 GMT
ADD file:5692a55e4805d33baa21e559cc0bb86fb91422171345ddd332fa5514285a3401 in / 
# Sat, 28 Dec 2019 05:03:25 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:10:52 GMT
ENV OTP_VERSION=19.3.6.13
# Sat, 28 Dec 2019 06:24:49 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="11a914176a33068226644f4e999ecc6e965ab1c60a324d90020f164641631fae" 	&& runtimeDeps=' 		libodbc1 		libssl1.0.2 		libsctp1 		libwxgtk3.0 	' 	&& buildDeps=' 		curl 		ca-certificates 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl1.0-dev 		libsctp-dev 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256 otp-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/otp-src 	&& tar -xzf otp-src.tar.gz -C /usr/src/otp-src --strip-components=1 	&& rm otp-src.tar.gz 	&& cd /usr/src/otp-src 	&& ./otp_build autoconf 	&& gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	&& ./configure --build="$gnuArch" 		--enable-dirty-schedulers 	&& make -j$(nproc) 	&& make install 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/otp-src /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:24:51 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:b531ae4a39253d883a11291e842b7e1aa9dae38f9d9b77ddea55b2625ce986e3`  
		Last Modified: Sat, 28 Dec 2019 05:10:53 GMT  
		Size: 42.1 MB (42108124 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c53022778c69df1b31bacb065494d17180051038a80dda2ec06dc60855c259c8`  
		Last Modified: Sat, 28 Dec 2019 06:36:06 GMT  
		Size: 200.7 MB (200734408 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:19-slim` - linux; arm64 variant v8

```console
$ docker pull erlang@sha256:e8d44b4e9c2f417a9a13567100ba647be7d0ced527e49361998cc4be0403a7b2
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **248.8 MB (248797299 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88a0cbba637c506c797fa2830b14d191e776345b243665a23756917e9636ed57`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:15 GMT
ADD file:e439b3c387852978811a6a5a058745ebb9392da7e8936beb4f37ff076e656213 in / 
# Sat, 28 Dec 2019 04:43:17 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 07:34:20 GMT
ENV OTP_VERSION=19.3.6.13
# Sat, 28 Dec 2019 07:46:41 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="11a914176a33068226644f4e999ecc6e965ab1c60a324d90020f164641631fae" 	&& runtimeDeps=' 		libodbc1 		libssl1.0.2 		libsctp1 		libwxgtk3.0 	' 	&& buildDeps=' 		curl 		ca-certificates 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl1.0-dev 		libsctp-dev 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256 otp-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/otp-src 	&& tar -xzf otp-src.tar.gz -C /usr/src/otp-src --strip-components=1 	&& rm otp-src.tar.gz 	&& cd /usr/src/otp-src 	&& ./otp_build autoconf 	&& gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	&& ./configure --build="$gnuArch" 		--enable-dirty-schedulers 	&& make -j$(nproc) 	&& make install 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/otp-src /var/lib/apt/lists/*
# Sat, 28 Dec 2019 07:46:48 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:d07bcf5901dfa793fa6b2c4c617e86bcef315b0b092cbfd1a929eefedaf8e3f2`  
		Last Modified: Sat, 28 Dec 2019 04:48:57 GMT  
		Size: 43.2 MB (43166476 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6cb7d466605e69eac3f3059b9942d322ad041f02ff2c7d6debacab60f4d603`  
		Last Modified: Sat, 28 Dec 2019 08:12:32 GMT  
		Size: 205.6 MB (205630823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:19-slim` - linux; 386

```console
$ docker pull erlang@sha256:6bf1797cbb62ce62cdd6989b07317d4f3009a32cf29461188d2b8e390e465c19
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.6 MB (259554407 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:10c98081a20fffa028f43adf2e7a629d3532809b7483c231a1b2533106d184fa`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:51 GMT
ADD file:f348ed8c5f7efee9f7e88d9a9bd1d57bca1bf445d486996cb6168da85c0bd43b in / 
# Sat, 28 Dec 2019 04:41:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:02:25 GMT
ENV OTP_VERSION=19.3.6.13
# Sat, 28 Dec 2019 08:21:14 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="11a914176a33068226644f4e999ecc6e965ab1c60a324d90020f164641631fae" 	&& runtimeDeps=' 		libodbc1 		libssl1.0.2 		libsctp1 		libwxgtk3.0 	' 	&& buildDeps=' 		curl 		ca-certificates 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl1.0-dev 		libsctp-dev 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256 otp-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/otp-src 	&& tar -xzf otp-src.tar.gz -C /usr/src/otp-src --strip-components=1 	&& rm otp-src.tar.gz 	&& cd /usr/src/otp-src 	&& ./otp_build autoconf 	&& gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	&& ./configure --build="$gnuArch" 		--enable-dirty-schedulers 	&& make -j$(nproc) 	&& make install 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/otp-src /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:21:14 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:410821d7ff8b427b8dfb93dcf31b1836a617f5c09be71f83a16ef2c5946ee700`  
		Last Modified: Sat, 28 Dec 2019 04:47:20 GMT  
		Size: 46.1 MB (46100094 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eca71cb24d011d9a699278d7b76ca59f76e3f0a2f34e71756290b383c1085630`  
		Last Modified: Sat, 28 Dec 2019 08:47:47 GMT  
		Size: 213.5 MB (213454313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `erlang:19-slim` - linux; s390x

```console
$ docker pull erlang@sha256:079af56667e4993dbf75e222c0e2f3cd5bc6e6c7c83e2eab2216638b3bd0b57d
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **259.3 MB (259292902 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:820e1a61bdb85b3d4581516d5555c3fe824a123eee127e93f4b48a0c6ce28845`
-	Default Command: `["erl"]`

```dockerfile
# Sat, 28 Dec 2019 04:43:08 GMT
ADD file:b85ece7344f0ad0749b115e76a51a3b9f322e23bcc8c692cd2edff403ba8840e in / 
# Sat, 28 Dec 2019 04:43:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 06:33:56 GMT
ENV OTP_VERSION=19.3.6.13
# Sat, 28 Dec 2019 06:39:50 GMT
RUN set -xe 	&& OTP_DOWNLOAD_URL="https://github.com/erlang/otp/archive/OTP-${OTP_VERSION}.tar.gz" 	&& OTP_DOWNLOAD_SHA256="11a914176a33068226644f4e999ecc6e965ab1c60a324d90020f164641631fae" 	&& runtimeDeps=' 		libodbc1 		libssl1.0.2 		libsctp1 		libwxgtk3.0 	' 	&& buildDeps=' 		curl 		ca-certificates 		autoconf 		dpkg-dev 		gcc 		g++ 		make 		libncurses-dev 		unixodbc-dev 		libssl1.0-dev 		libsctp-dev 	' 	&& apt-get update 	&& apt-get install -y --no-install-recommends $runtimeDeps 	&& apt-get install -y --no-install-recommends $buildDeps 	&& curl -fSL -o otp-src.tar.gz "$OTP_DOWNLOAD_URL" 	&& echo "$OTP_DOWNLOAD_SHA256 otp-src.tar.gz" | sha256sum -c - 	&& mkdir -p /usr/src/otp-src 	&& tar -xzf otp-src.tar.gz -C /usr/src/otp-src --strip-components=1 	&& rm otp-src.tar.gz 	&& cd /usr/src/otp-src 	&& ./otp_build autoconf 	&& gnuArch="$(dpkg-architecture --query DEB_HOST_GNU_TYPE)" 	&& ./configure --build="$gnuArch" 		--enable-dirty-schedulers 	&& make -j$(nproc) 	&& make install 	&& find /usr/local -name examples | xargs rm -rf 	&& apt-get purge -y --auto-remove $buildDeps 	&& rm -rf /usr/src/otp-src /var/lib/apt/lists/*
# Sat, 28 Dec 2019 06:39:51 GMT
CMD ["erl"]
```

-	Layers:
	-	`sha256:5bf261872a9b22035011c2bf77259c73389d0d5786e4b43bee1df89b5dfada2f`  
		Last Modified: Sat, 28 Dec 2019 04:46:24 GMT  
		Size: 45.2 MB (45241644 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34bd28a3e0490d9ed7e95044ce572f64ce28c54dd0e494a08a7c18eea469f9df`  
		Last Modified: Sat, 28 Dec 2019 06:52:09 GMT  
		Size: 214.1 MB (214051258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
