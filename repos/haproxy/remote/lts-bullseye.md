## `haproxy:lts-bullseye`

```console
$ docker pull haproxy@sha256:f3afb16079cfa3801b40d3d64c7780a5b33a67cb7294246265d5f5d19b3494ab
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

### `haproxy:lts-bullseye` - linux; amd64

```console
$ docker pull haproxy@sha256:9a98def69ec51204ca8f202c3c0d442e1732707a6dbe61b77b417b06fad60cba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.1 MB (39122064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a68ae3ea0e3def26dab4ad848f224d3e3e2c0dcef5704a045e6416bf433bb236`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 12 Oct 2021 01:20:42 GMT
ADD file:16dc2c6d1932194edec28d730b004fd6deca3d0f0e1a07bc5b8b6e8a1662f7af in / 
# Tue, 12 Oct 2021 01:20:42 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:18:48 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 03 Nov 2021 19:24:21 GMT
ENV HAPROXY_VERSION=2.4.8
# Wed, 03 Nov 2021 19:24:22 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.8.tar.gz
# Wed, 03 Nov 2021 19:24:22 GMT
ENV HAPROXY_SHA256=e3e4c1ad293bc25e8d8790cc5e45133213dda008bfd0228bf3077259b32ebaa5
# Wed, 03 Nov 2021 19:25:13 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 03 Nov 2021 19:25:13 GMT
STOPSIGNAL SIGUSR1
# Wed, 03 Nov 2021 19:25:13 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 03 Nov 2021 19:25:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Nov 2021 19:25:13 GMT
USER haproxy
# Wed, 03 Nov 2021 19:25:14 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:7d63c13d9b9b6ec5f05a2b07daadacaa9c610d01102a662ae9b1d082105f1ffa`  
		Last Modified: Tue, 12 Oct 2021 01:26:05 GMT  
		Size: 31.4 MB (31357311 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca14c2a724ffea2ec5059f2880fce4d9b508ed025a1e74b839d2d8b4c60f1665`  
		Last Modified: Tue, 12 Oct 2021 09:27:05 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ceabb6fa5dbb68f3757782f0c30dd191e4fb6a0d17e53c41447ad6e5d5a15e17`  
		Last Modified: Wed, 03 Nov 2021 19:28:15 GMT  
		Size: 7.8 MB (7762866 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3349425285d32f50c47f5845a1ff6a01f131cd51dc62b69310ca87d848c049fb`  
		Last Modified: Wed, 03 Nov 2021 19:28:14 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-bullseye` - linux; arm variant v5

```console
$ docker pull haproxy@sha256:e53820cff6b1955ab9203a88e5dbe2b28e78ad5f65bdd002129de718563c016f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **36.6 MB (36577920 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:71655810d7fac60dc5220e83ce4d74fc2f6f04ac34e8da2a3512dfde3283652a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 12 Oct 2021 00:50:30 GMT
ADD file:fb1afabdc1f93b4866b4c4d696f272b4888519cb5bf35eb7ed1a4c021d1a04c8 in / 
# Tue, 12 Oct 2021 00:50:30 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:15:51 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 03 Nov 2021 19:49:56 GMT
ENV HAPROXY_VERSION=2.4.8
# Wed, 03 Nov 2021 19:49:56 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.8.tar.gz
# Wed, 03 Nov 2021 19:49:56 GMT
ENV HAPROXY_SHA256=e3e4c1ad293bc25e8d8790cc5e45133213dda008bfd0228bf3077259b32ebaa5
# Wed, 03 Nov 2021 19:50:50 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 03 Nov 2021 19:50:51 GMT
STOPSIGNAL SIGUSR1
# Wed, 03 Nov 2021 19:50:52 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 03 Nov 2021 19:50:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Nov 2021 19:50:53 GMT
USER haproxy
# Wed, 03 Nov 2021 19:50:54 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:5c9bab66abc5c53391435f6fd66e0ff3571295d568f45ac7d2dc480bcbfd56e8`  
		Last Modified: Tue, 12 Oct 2021 01:06:07 GMT  
		Size: 28.9 MB (28899715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6729bc13bbc97dcc43292017b35f3ea0e7d283d3179c431bb5013521155f4bcd`  
		Last Modified: Tue, 12 Oct 2021 06:26:26 GMT  
		Size: 1.4 KB (1436 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bec81c2fc3853363c4c9f25476ad97c97bad9d7990ec5ad3fa1ab9e60b72f1ce`  
		Last Modified: Wed, 03 Nov 2021 19:54:58 GMT  
		Size: 7.7 MB (7676314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9f37ade413028403faa1d55e2975e2853ba4765504b6bc5fe895e8264e3cbc22`  
		Last Modified: Wed, 03 Nov 2021 19:54:53 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-bullseye` - linux; arm variant v7

```console
$ docker pull haproxy@sha256:e88c0b256e94b62b9a3239017a3765c0f33d5770f53a1c013b81b088908c9450
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.1 MB (34092043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0262a09aef8d8bf9b5e6c4657bdf3c825f975ca95d282a38734b2b71475c22bb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 12 Oct 2021 01:28:36 GMT
ADD file:89eac94007ac04f9168737686fa0a6c737f2c28fc9e5918d4d512924fe1973be in / 
# Tue, 12 Oct 2021 01:28:37 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 05:27:01 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 12 Oct 2021 05:28:19 GMT
ENV HAPROXY_VERSION=2.4.7
# Tue, 12 Oct 2021 05:28:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.7.tar.gz
# Tue, 12 Oct 2021 05:28:20 GMT
ENV HAPROXY_SHA256=52af97f72f22ffd8a7a995fafc696291d37818feda50a23caef7dc0622421845
# Tue, 12 Oct 2021 05:29:08 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 12 Oct 2021 05:29:08 GMT
STOPSIGNAL SIGUSR1
# Tue, 12 Oct 2021 05:29:09 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 12 Oct 2021 05:29:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 05:29:10 GMT
USER haproxy
# Tue, 12 Oct 2021 05:29:10 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:4e5300249f84466df4dc73ea0ce09938ca00c1718bb12619c4f26bd936162331`  
		Last Modified: Tue, 12 Oct 2021 01:44:28 GMT  
		Size: 26.6 MB (26561058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6af400fcb60ee6023eb9564d98a626de263d2b1f72541c2c9e831bd08f0bb807`  
		Last Modified: Tue, 12 Oct 2021 05:40:41 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43f31871ad82103f3bd51eca101fe6b9678155ce94633d59fbbab5edbe98b10`  
		Last Modified: Tue, 12 Oct 2021 05:41:15 GMT  
		Size: 7.5 MB (7529099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bef86ed5e712feb8f32b1621dc4ae1dcb3e56af0428b2488453fcbea19548044`  
		Last Modified: Tue, 12 Oct 2021 05:41:11 GMT  
		Size: 455.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-bullseye` - linux; arm64 variant v8

```console
$ docker pull haproxy@sha256:770d951f86ffc4dcb3384571df0f1d84f65f941c9c10c7f9cbc4b7618cb93a9b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.9 MB (37853644 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:69e66535468318eba7559f8019915c421cc0f1b13e0539aeec170b453aa36d62`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 12 Oct 2021 01:41:18 GMT
ADD file:d84144ad575672cd6cc8a00c8e5a88ab0545348f040fc249ea5fcf8193b2bce6 in / 
# Tue, 12 Oct 2021 01:41:18 GMT
CMD ["bash"]
# Mon, 18 Oct 2021 22:06:29 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 03 Nov 2021 19:57:19 GMT
ENV HAPROXY_VERSION=2.4.8
# Wed, 03 Nov 2021 19:57:20 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.8.tar.gz
# Wed, 03 Nov 2021 19:57:21 GMT
ENV HAPROXY_SHA256=e3e4c1ad293bc25e8d8790cc5e45133213dda008bfd0228bf3077259b32ebaa5
# Wed, 03 Nov 2021 19:57:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 03 Nov 2021 19:57:51 GMT
STOPSIGNAL SIGUSR1
# Wed, 03 Nov 2021 19:57:53 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 03 Nov 2021 19:57:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Nov 2021 19:57:54 GMT
USER haproxy
# Wed, 03 Nov 2021 19:57:55 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:a9eb63951c1c2ee8efcc12b696928fee3741a2d4eae76f2da3e161a5d90548bf`  
		Last Modified: Tue, 12 Oct 2021 01:48:13 GMT  
		Size: 30.0 MB (30043906 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc1f98bac462b4adfaa59a33c74144d7cbc0a5d780052262d06d22aaf6df0fe9`  
		Last Modified: Mon, 18 Oct 2021 22:17:34 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7a24c35f70c35e00a06f3cd94b5861511ec12b4d59989c41b7f37fca3682fa1`  
		Last Modified: Wed, 03 Nov 2021 20:02:12 GMT  
		Size: 7.8 MB (7807998 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e23357b6a7df0be2769f0bbe150c7ae6a812ab8622e81d778bf2ca29bc9240f`  
		Last Modified: Wed, 03 Nov 2021 20:02:10 GMT  
		Size: 453.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-bullseye` - linux; 386

```console
$ docker pull haproxy@sha256:00bc7b84593393c9aa015e74384c47a22d211b9a9a62807c439f5c6b5a8bec77
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.9 MB (39904166 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ae421a0bb30ef5fe6776bba4c0ad7482ca4bd34fba2e0ba779e95c3a543dd07`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 12 Oct 2021 01:39:47 GMT
ADD file:42196ffa4c70af8d9f1e7b74edb3bb92d47296acf989adf615e8208230f8bd0c in / 
# Tue, 12 Oct 2021 01:39:47 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 09:30:49 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 12 Oct 2021 09:32:18 GMT
ENV HAPROXY_VERSION=2.4.7
# Tue, 12 Oct 2021 09:32:19 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.7.tar.gz
# Tue, 12 Oct 2021 09:32:19 GMT
ENV HAPROXY_SHA256=52af97f72f22ffd8a7a995fafc696291d37818feda50a23caef7dc0622421845
# Tue, 12 Oct 2021 09:33:24 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 12 Oct 2021 09:33:24 GMT
STOPSIGNAL SIGUSR1
# Tue, 12 Oct 2021 09:33:24 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 12 Oct 2021 09:33:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 09:33:25 GMT
USER haproxy
# Tue, 12 Oct 2021 09:33:25 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:87318d165b5c0fdf05c8ccf97d83084f56b4608075a3335b1a46c76295b82753`  
		Last Modified: Tue, 12 Oct 2021 01:47:39 GMT  
		Size: 32.4 MB (32370344 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b812a1b16a1ab832fcaac2acc742227bee1503a26ab2a6d70293765b3ba80566`  
		Last Modified: Tue, 12 Oct 2021 09:42:17 GMT  
		Size: 1.4 KB (1429 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b50917b26fb5b5defe5bcb5be18386059578805364dd2605860664a3868bd5`  
		Last Modified: Tue, 12 Oct 2021 09:42:42 GMT  
		Size: 7.5 MB (7531939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8f6b28a6494ba9a1738f7cdb4fbe8d54607c62ac2d0fc2780ede4367e547048`  
		Last Modified: Tue, 12 Oct 2021 09:42:40 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-bullseye` - linux; mips64le

```console
$ docker pull haproxy@sha256:763aa5ee10d1c1a6d47ca5b317374fb2775b06b1057c8978a6e8d98a8c3d091e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.5 MB (37521322 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:50a3362490d1e911b8c568a002c2893c9d16179abdfe3f0c775c33cc52cd98c2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 12 Oct 2021 01:11:15 GMT
ADD file:f90ca8957172106f42a9096c9a21082d51f3201aa78e6f64621a73117e2b7b6a in / 
# Tue, 12 Oct 2021 01:11:16 GMT
CMD ["bash"]
# Wed, 13 Oct 2021 01:10:12 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 03 Nov 2021 19:13:12 GMT
ENV HAPROXY_VERSION=2.4.8
# Wed, 03 Nov 2021 19:13:12 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.8.tar.gz
# Wed, 03 Nov 2021 19:13:12 GMT
ENV HAPROXY_SHA256=e3e4c1ad293bc25e8d8790cc5e45133213dda008bfd0228bf3077259b32ebaa5
# Wed, 03 Nov 2021 19:15:46 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 03 Nov 2021 19:15:46 GMT
STOPSIGNAL SIGUSR1
# Wed, 03 Nov 2021 19:15:47 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 03 Nov 2021 19:15:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Nov 2021 19:15:47 GMT
USER haproxy
# Wed, 03 Nov 2021 19:15:48 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:59ddca50ce05605e6234c1e7213c39cdedabc48ef11637e12156b7bd69afe161`  
		Last Modified: Tue, 12 Oct 2021 01:20:03 GMT  
		Size: 29.6 MB (29618732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1a3ce348fb895deb27174246ab67920b8738280548ff0a113d108514f9034f1b`  
		Last Modified: Wed, 13 Oct 2021 01:27:36 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5590379403a73cc6b0383549e8e41a2dcc99e6970bae531a5ce0f8cd8a7a5b6`  
		Last Modified: Wed, 03 Nov 2021 19:17:07 GMT  
		Size: 7.9 MB (7900728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4d8a56449900dfbf2bda8a9900fd0328cfea81308689a00a4a2727f781bb1f0`  
		Last Modified: Wed, 03 Nov 2021 19:17:01 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-bullseye` - linux; ppc64le

```console
$ docker pull haproxy@sha256:4b8c3a3b8adb68a4f711cda8f0cbdb5691cfe5cdf7eb08b7059d55c73429c74f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43406169 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a251ac00422ba427685d92dd164974177b1658aa5fed49c3f8da2f3c1fc81a0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 12 Oct 2021 01:25:45 GMT
ADD file:d8794fadf16c9948c3574ba28740d08393eca57766340333ad91f9c2a33eb719 in / 
# Tue, 12 Oct 2021 01:25:53 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 06:20:14 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Tue, 12 Oct 2021 06:23:05 GMT
ENV HAPROXY_VERSION=2.4.7
# Tue, 12 Oct 2021 06:23:08 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.7.tar.gz
# Tue, 12 Oct 2021 06:23:10 GMT
ENV HAPROXY_SHA256=52af97f72f22ffd8a7a995fafc696291d37818feda50a23caef7dc0622421845
# Tue, 12 Oct 2021 06:26:17 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Tue, 12 Oct 2021 06:26:19 GMT
STOPSIGNAL SIGUSR1
# Tue, 12 Oct 2021 06:26:22 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Tue, 12 Oct 2021 06:26:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 12 Oct 2021 06:26:27 GMT
USER haproxy
# Tue, 12 Oct 2021 06:26:32 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:6c28c1405c677dd809094d06190225b38cee3d24f18da38d287ef5bcc67884d6`  
		Last Modified: Tue, 12 Oct 2021 01:37:00 GMT  
		Size: 35.3 MB (35258729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db70adf0ef6d4b0f81c247086b65a0ecd408f37b299a392560d9860f408cec20`  
		Last Modified: Tue, 12 Oct 2021 06:47:11 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:831499a44430c71ebce5bd98d3712f04228a9c8bec890e233aba98a867c869b8`  
		Last Modified: Tue, 12 Oct 2021 06:47:33 GMT  
		Size: 8.1 MB (8145551 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0b02a1d933e4263b6a352f77d73a5be3240f533d923f76f95966246f9278b9b`  
		Last Modified: Tue, 12 Oct 2021 06:47:31 GMT  
		Size: 454.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `haproxy:lts-bullseye` - linux; s390x

```console
$ docker pull haproxy@sha256:58beffa49e8378859d54d8b1f7f18859b8b2f8a62836794da96045dfc2cab29c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.5 MB (37451247 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f66cafc09e69509c1993ff00e6c176290b47fb059de4862935139309c310d0dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["haproxy","-f","\/usr\/local\/etc\/haproxy\/haproxy.cfg"]`

```dockerfile
# Tue, 12 Oct 2021 00:42:27 GMT
ADD file:6038dd6db57fb05c3d39c02c3379667ccd2989e7667ff773a8020fe6a69a760c in / 
# Tue, 12 Oct 2021 00:42:29 GMT
CMD ["bash"]
# Tue, 12 Oct 2021 07:29:02 GMT
RUN set -eux; 	groupadd --gid 99 --system haproxy; 	useradd 		--gid haproxy 		--home-dir /var/lib/haproxy 		--no-create-home 		--system 		--uid 99 		haproxy 	; 	mkdir /var/lib/haproxy; 	chown haproxy:haproxy /var/lib/haproxy
# Wed, 03 Nov 2021 19:47:09 GMT
ENV HAPROXY_VERSION=2.4.8
# Wed, 03 Nov 2021 19:47:09 GMT
ENV HAPROXY_URL=https://www.haproxy.org/download/2.4/src/haproxy-2.4.8.tar.gz
# Wed, 03 Nov 2021 19:47:09 GMT
ENV HAPROXY_SHA256=e3e4c1ad293bc25e8d8790cc5e45133213dda008bfd0228bf3077259b32ebaa5
# Wed, 03 Nov 2021 19:47:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update && apt-get install -y --no-install-recommends 		ca-certificates 		gcc 		libc6-dev 		liblua5.3-dev 		libpcre2-dev 		libssl-dev 		make 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O haproxy.tar.gz "$HAPROXY_URL"; 	echo "$HAPROXY_SHA256 *haproxy.tar.gz" | sha256sum -c; 	mkdir -p /usr/src/haproxy; 	tar -xzf haproxy.tar.gz -C /usr/src/haproxy --strip-components=1; 	rm haproxy.tar.gz; 		makeOpts=' 		TARGET=linux-glibc 		USE_GETADDRINFO=1 		USE_LUA=1 LUA_INC=/usr/include/lua5.3 		USE_OPENSSL=1 		USE_PCRE2=1 USE_PCRE2_JIT=1 		USE_PROMEX=1 				EXTRA_OBJS=" 		" 	'; 	dpkgArch="$(dpkg --print-architecture)"; 	case "$dpkgArch" in 		armel) makeOpts="$makeOpts ADDLIB=-latomic" ;; 	esac; 		nproc="$(nproc)"; 	eval "make -C /usr/src/haproxy -j '$nproc' all $makeOpts"; 	eval "make -C /usr/src/haproxy install-bin $makeOpts"; 		mkdir -p /usr/local/etc/haproxy; 	cp -R /usr/src/haproxy/examples/errorfiles /usr/local/etc/haproxy/errors; 	rm -rf /usr/src/haproxy; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		haproxy -v
# Wed, 03 Nov 2021 19:47:38 GMT
STOPSIGNAL SIGUSR1
# Wed, 03 Nov 2021 19:47:38 GMT
COPY file:a7db5ef8dbcd831ff68d6ff2fb45bc340539ad6d7a58d54323fd7399d1520910 in /usr/local/bin/ 
# Wed, 03 Nov 2021 19:47:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 Nov 2021 19:47:38 GMT
USER haproxy
# Wed, 03 Nov 2021 19:47:38 GMT
CMD ["haproxy" "-f" "/usr/local/etc/haproxy/haproxy.cfg"]
```

-	Layers:
	-	`sha256:ded751c48f72503973be01be2794cc039490f22b039b8ac106e9f17de4980742`  
		Last Modified: Tue, 12 Oct 2021 00:48:05 GMT  
		Size: 29.6 MB (29641215 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5df628207bd790253fb56f38c6d2e8ef8f56a352db7ae6304c74e06c24787255`  
		Last Modified: Tue, 12 Oct 2021 07:35:33 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f07791dc59f66d14056c055209f5b4b9d08a316ccd276bad1cffacd1fd45dc54`  
		Last Modified: Wed, 03 Nov 2021 19:52:07 GMT  
		Size: 7.8 MB (7808143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54a5a43e875a539fbd0823a1231f5924a66a35938fb721f3afeceae3658af29a`  
		Last Modified: Wed, 03 Nov 2021 19:52:02 GMT  
		Size: 456.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
