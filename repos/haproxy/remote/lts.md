## `haproxy:lts`

```console
$ docker pull haproxy@sha256:46b76a587df7d43c587178cbbed2cbcc0781a8d2b6f5fc4dd4f8f4706416461d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 8
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; mips64le
	-	linux; ppc64le
	-	linux; s390x

### `haproxy:lts` - linux; amd64

```console
$ docker pull haproxy@sha256:8da4a97c4a5ebbd076d8287048a385d314116167162a20c4ed8be5c97e6ddfc2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.1 MB (40138696 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b65a9804e8c5221b429533abf86b18d7c50a437824c14ee942c8f937f5dc1e31`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:58 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 21 Nov 2023 05:21:58 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 13:10:54 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 07 Dec 2023 22:19:50 GMT
ENV HAPROXY_VERSION=2.8.5
# Thu, 07 Dec 2023 22:19:50 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Thu, 07 Dec 2023 22:19:50 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
# Thu, 07 Dec 2023 22:20:29 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 07 Dec 2023 22:20:29 GMT
STOPSIGNAL SIGUSR1
# Thu, 07 Dec 2023 22:20:29 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 07 Dec 2023 22:20:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:20:30 GMT
USER haproxy
# Thu, 07 Dec 2023 22:20:30 GMT
WORKDIR /var/lib/haproxy
# Thu, 07 Dec 2023 22:20:30 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1bbaaca6e72727d1473cab3ef6beb3a1ef3dbae7a979632f9c7c06dad32e9c90`  
		Last Modified: Tue, 21 Nov 2023 13:16:35 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f26af61f54d75bc45f92d0a5acbde0cf899e9342b0a8752c5a934dd9e0418ef`  
		Last Modified: Thu, 07 Dec 2023 22:23:43 GMT  
		Size: 8.7 MB (8718984 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7e8f787f6102e250459f7be9502e56fae6287a505c5fa1b1375bcebdbcd0e0a`  
		Last Modified: Thu, 07 Dec 2023 22:23:41 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:066cef0eee9f7423b3cf13fb6709ea10ebbf59ccb8d45006a1c19da8fbe5f61c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.5 MB (37520772 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c9f0a10df9dd1cff386356d83d514f0407e334d974a5458549e8c06eef3fef1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 05:01:09 GMT
ADD file:f7d1d017cc4e588f213f4536967b8d58c50b8602fb8a10b786856c35a843f31e in / 
# Tue, 21 Nov 2023 05:01:09 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 06:04:32 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 07 Dec 2023 21:48:20 GMT
ENV HAPROXY_VERSION=2.8.5
# Thu, 07 Dec 2023 21:48:21 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Thu, 07 Dec 2023 21:48:21 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
# Thu, 07 Dec 2023 21:48:59 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 07 Dec 2023 21:48:59 GMT
STOPSIGNAL SIGUSR1
# Thu, 07 Dec 2023 21:48:59 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:48:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:48:59 GMT
USER haproxy
# Thu, 07 Dec 2023 21:48:59 GMT
WORKDIR /var/lib/haproxy
# Thu, 07 Dec 2023 21:48:59 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:d051266714ac5508b442ebbe5911d353bfacddc64f657eeba14a993cced96358`  
		Last Modified: Tue, 21 Nov 2023 05:04:38 GMT  
		Size: 28.9 MB (28921267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03bff403e67bc579e6982f56000a9281d8baa40442fb5c9cb616649bdaa489aa`  
		Last Modified: Tue, 21 Nov 2023 06:09:16 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05df80614e5d19e367c510d5aa895cde1ba5f03da242053514631b912e8673d2`  
		Last Modified: Thu, 07 Dec 2023 21:50:26 GMT  
		Size: 8.6 MB (8597618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:166185370a529ff0265903a483c34c9b13440cc90ea8ec2daca2d905ab0fb4e2`  
		Last Modified: Thu, 07 Dec 2023 21:50:25 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:1c2119a4ae36b1d40c6521425ab6326d42a26e4f7469aaa0e20f4249b9191dd0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (35031117 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f74d6c1850658cfda08bbba1d62a7bab05078973c9ee9e7e17a2ab5704b17c32`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 03:58:04 GMT
ADD file:c4afced274aaa80ab3018b368ed739c1c55e49b41e9637ac44d63e61344fe865 in / 
# Tue, 21 Nov 2023 03:58:04 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 13:56:41 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 07 Dec 2023 21:57:30 GMT
ENV HAPROXY_VERSION=2.8.5
# Thu, 07 Dec 2023 21:57:30 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Thu, 07 Dec 2023 21:57:30 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
# Thu, 07 Dec 2023 21:58:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 07 Dec 2023 21:58:01 GMT
STOPSIGNAL SIGUSR1
# Thu, 07 Dec 2023 21:58:01 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:58:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:58:01 GMT
USER haproxy
# Thu, 07 Dec 2023 21:58:01 GMT
WORKDIR /var/lib/haproxy
# Thu, 07 Dec 2023 21:58:02 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6dc4ed5513793308b8e30b08e03f97fa54025c3d3f3172c6edccb1dbbc7ff139`  
		Last Modified: Tue, 21 Nov 2023 04:02:35 GMT  
		Size: 26.6 MB (26579014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecd7b216a08b31174ea7ba0d1723b8df8b1a3fc7bcdf5fb6295c87ec5ff489c`  
		Last Modified: Tue, 21 Nov 2023 14:01:41 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:551cef44ce9ff0d248ccf7178dce42e138a056a132936ec773aa97445f7c3894`  
		Last Modified: Thu, 07 Dec 2023 22:00:38 GMT  
		Size: 8.5 MB (8450220 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba1bf8b8949709d5e359ad104ff379fb39c85e9cdf5ddcd17f330825a6aa265d`  
		Last Modified: Thu, 07 Dec 2023 22:00:37 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:5c990f85de5b74cf7c6ad688ad072a3909b189a7302ef2d105b2a766d7f72494
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38760642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f10e47b95496f1a97c8c3cbf473a3ef36e049b81ae6fe4ebf9ae369ef0ca0dc5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 08:56:45 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 07 Dec 2023 21:39:42 GMT
ENV HAPROXY_VERSION=2.8.5
# Thu, 07 Dec 2023 21:39:42 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Thu, 07 Dec 2023 21:39:43 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
# Thu, 07 Dec 2023 21:40:10 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 07 Dec 2023 21:40:10 GMT
STOPSIGNAL SIGUSR1
# Thu, 07 Dec 2023 21:40:10 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:40:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:40:10 GMT
USER haproxy
# Thu, 07 Dec 2023 21:40:10 GMT
WORKDIR /var/lib/haproxy
# Thu, 07 Dec 2023 21:40:10 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bde50ca79c16a524ea15fa642818165d9cbf25225f563d20df794d5e6dd70713`  
		Last Modified: Tue, 21 Nov 2023 09:00:46 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3928f93ce48821e6b714e385e520c2ab9c6783b4e42bc2ff210ea482605a92f1`  
		Last Modified: Thu, 07 Dec 2023 21:42:26 GMT  
		Size: 8.7 MB (8694627 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:acda15d594c89c65eaac562e67ad182cb0fe3329f3fc09ec39a7467e050843ff`  
		Last Modified: Thu, 07 Dec 2023 21:42:25 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; 386

```console
$ docker pull haproxy@sha256:87de1626299052bb2774dd110b84a7f0a37c09e104e6fbb058a6ef0fe1df7233
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.9 MB (40874624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:211dc015908ed727ffdcc1810e3df219072aadc9dac71fc60087818d79fdaaca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:15 GMT
ADD file:7de881b584405a880c4d02778056aaa81bb5dd5d1af65b3086d66aed9ff0ad4b in / 
# Tue, 21 Nov 2023 04:40:16 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 16:01:16 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 07 Dec 2023 21:38:28 GMT
ENV HAPROXY_VERSION=2.8.5
# Thu, 07 Dec 2023 21:38:28 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Thu, 07 Dec 2023 21:38:28 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
# Thu, 07 Dec 2023 21:39:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 07 Dec 2023 21:39:36 GMT
STOPSIGNAL SIGUSR1
# Thu, 07 Dec 2023 21:39:36 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:39:37 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:39:37 GMT
USER haproxy
# Thu, 07 Dec 2023 21:39:37 GMT
WORKDIR /var/lib/haproxy
# Thu, 07 Dec 2023 21:39:37 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:75c11612678b54e79a38118fe66e532c61b3d0798afb741007b4cd3209c0ec4e`  
		Last Modified: Tue, 21 Nov 2023 04:45:24 GMT  
		Size: 32.4 MB (32402632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21862fb0fc1c2fb072bdb6e21122d3878b6eae0894075d5c8df68954704adf01`  
		Last Modified: Tue, 21 Nov 2023 16:10:16 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c4c13f9fcfc2d5307fe2ffe21b7626342615060d1330220074685ce199b9583`  
		Last Modified: Thu, 07 Dec 2023 21:44:27 GMT  
		Size: 8.5 MB (8470106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11725dce133c63f983ab88a167083bfd4f13474112299ae7dc7fff4962620712`  
		Last Modified: Thu, 07 Dec 2023 21:44:25 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; mips64le

```console
$ docker pull haproxy@sha256:7f31619740dc7a2fe2dae5ef3398b1d0c9fb103f04acad93178c22cad04b7329
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38439787 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:874014c5c6508883224335f0087dc289249434e1eb5ab23d516becd5615e389d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 04:11:02 GMT
ADD file:09d1c4f0f5b78b81f635498ee58f6ab1843bca8a18549ecc39686f1c60b1951d in / 
# Tue, 21 Nov 2023 04:11:06 GMT
CMD ["bash"]
# Wed, 22 Nov 2023 06:59:03 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 07 Dec 2023 22:07:46 GMT
ENV HAPROXY_VERSION=2.8.5
# Thu, 07 Dec 2023 22:07:49 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Thu, 07 Dec 2023 22:07:51 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
# Thu, 07 Dec 2023 22:11:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 07 Dec 2023 22:11:28 GMT
STOPSIGNAL SIGUSR1
# Thu, 07 Dec 2023 22:11:30 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 07 Dec 2023 22:11:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:11:34 GMT
USER haproxy
# Thu, 07 Dec 2023 22:11:37 GMT
WORKDIR /var/lib/haproxy
# Thu, 07 Dec 2023 22:11:39 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a157b7f5d72df9473d33b22278cb42e4e06e22b99ac1864b7b586f36671f15bb`  
		Last Modified: Tue, 21 Nov 2023 04:22:02 GMT  
		Size: 29.6 MB (29636034 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c96ff252242aad32681033b4b6b93ef2f1ce05092379c1ff7990431632bd286`  
		Last Modified: Wed, 22 Nov 2023 07:22:44 GMT  
		Size: 1.3 KB (1293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8745c5f95fff2cdec3fd9993ec9fd618b6844b39528bb0e9d616383380845f2`  
		Last Modified: Thu, 07 Dec 2023 22:16:38 GMT  
		Size: 8.8 MB (8802006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f16c897294e47430b518b5916d512fd759c758798e0dca3cea53b3efc1654b4`  
		Last Modified: Thu, 07 Dec 2023 22:16:33 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; ppc64le

```console
$ docker pull haproxy@sha256:d914764ba6d747513a1e28ce99ccdaa688386a156949edf565f07d82ec4f2d59
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **44.4 MB (44444524 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:881955c23876d6bb8ae4c65fd8d49b197bcb8141bd2fa676f0504e30753c93a3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 07:59:09 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 07 Dec 2023 22:19:41 GMT
ENV HAPROXY_VERSION=2.8.5
# Thu, 07 Dec 2023 22:19:41 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Thu, 07 Dec 2023 22:19:41 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
# Thu, 07 Dec 2023 22:20:32 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 07 Dec 2023 22:20:32 GMT
STOPSIGNAL SIGUSR1
# Thu, 07 Dec 2023 22:20:32 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 07 Dec 2023 22:20:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 22:20:33 GMT
USER haproxy
# Thu, 07 Dec 2023 22:20:33 GMT
WORKDIR /var/lib/haproxy
# Thu, 07 Dec 2023 22:20:33 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2aafd76cec07be5fc8a0508a6a0b7241005c9e5273dc6081c67c74933c5033e`  
		Last Modified: Tue, 21 Nov 2023 08:04:43 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b89b073750b46a203f32daafdaa163d8bb370296e3c5e35609394f4070c87cc`  
		Last Modified: Thu, 07 Dec 2023 22:23:27 GMT  
		Size: 9.1 MB (9148909 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e0c2e21df1e9fcd1b7113add42a5e35076a7f96cef88a2c25a61568bea7d1661`  
		Last Modified: Thu, 07 Dec 2023 22:23:25 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts` - linux; s390x

```console
$ docker pull haproxy@sha256:de0630ac4eabf8c6cbaddae9869ceb4729c119fa152dd05ede06bf8cc4b52d5b
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.4 MB (38388250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58a54268aa7d020aa403fbf4f27f539743c719625574163e08c25b243edc93d2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 21 Nov 2023 05:05:18 GMT
ADD file:a545f27075704ce13e33e539170d3f47007424d2cc2bea5aecfd2608a5194151 in / 
# Tue, 21 Nov 2023 05:05:22 GMT
CMD ["bash"]
# Tue, 21 Nov 2023 05:33:11 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Thu, 07 Dec 2023 21:42:39 GMT
ENV HAPROXY_VERSION=2.8.5
# Thu, 07 Dec 2023 21:42:39 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.8/src/haproxy-2.8.5.tar.gz
# Thu, 07 Dec 2023 21:42:39 GMT
ENV HAPROXY_SHA256=3f5459c5a58e0b343a32eaef7ed5bed9d3fc29d8aa9e14b36c92c969fc2a60d9
# Thu, 07 Dec 2023 21:43:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Thu, 07 Dec 2023 21:43:18 GMT
STOPSIGNAL SIGUSR1
# Thu, 07 Dec 2023 21:43:18 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Thu, 07 Dec 2023 21:43:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 07 Dec 2023 21:43:19 GMT
USER haproxy
# Thu, 07 Dec 2023 21:43:19 GMT
WORKDIR /var/lib/haproxy
# Thu, 07 Dec 2023 21:43:19 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:b114072f1cab66b7376d690985b12816aebab2e4e41fc170e32f111df27951dc`  
		Last Modified: Tue, 21 Nov 2023 05:10:48 GMT  
		Size: 29.7 MB (29656938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4ea5b47f5f5ce48b0231eff62a313c71c777892df26e1a8c9e0b53f34ec2702`  
		Last Modified: Tue, 21 Nov 2023 05:38:46 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365eeacee7ebb55a015ce914c06f359d1322556cb85c1b56bc6e145eb403e9c8`  
		Last Modified: Thu, 07 Dec 2023 21:47:38 GMT  
		Size: 8.7 MB (8729425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d245b12584c05ffb0a08f2d46e0f1f4cd3f43bf6e819e6e0f148a1996bb2920`  
		Last Modified: Thu, 07 Dec 2023 21:47:35 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
