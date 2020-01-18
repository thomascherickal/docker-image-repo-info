<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `httpd`

-	[`httpd:2`](#httpd2)
-	[`httpd:2.4`](#httpd24)
-	[`httpd:2.4.41`](#httpd2441)
-	[`httpd:2.4.41-alpine`](#httpd2441-alpine)
-	[`httpd:2.4-alpine`](#httpd24-alpine)
-	[`httpd:2-alpine`](#httpd2-alpine)
-	[`httpd:alpine`](#httpdalpine)
-	[`httpd:latest`](#httpdlatest)

## `httpd:2`

```console
$ docker pull httpd@sha256:769018135ba22d3a7a2b91cb89b8de711562cdf51ad6621b2b9b13e95f3798de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `httpd:2` - linux; amd64

```console
$ docker pull httpd@sha256:63dbdd1b6cb325d3afda7774a068ad1c6658490d8d4cd505a4db9d927f9f9afc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.8 MB (61847101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2aa7e16edd855da8827aa0ccf976d1d50f0827c08622c16e0750aa1591717e5`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:08:55 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 13:08:55 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:08:57 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 13:08:57 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 13:09:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:09:05 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 13:09:06 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 13:09:06 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 13:13:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 13:13:36 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 13:13:37 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 13:13:37 GMT
EXPOSE 80
# Sat, 28 Dec 2019 13:13:37 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354e6904d6556707e95c6952df767d7e6447392700fa07d33cd673d28ed80329`  
		Last Modified: Sat, 28 Dec 2019 13:13:50 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27298e4c749a2e37d2842e5200bb388402405c04e2de9fb97a05c868c4df9f7b`  
		Last Modified: Sat, 28 Dec 2019 13:13:53 GMT  
		Size: 10.4 MB (10374093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e27104ba69adc141aa1d84510fd98ae550036abd7a02d4a8881152d18f3aa2`  
		Last Modified: Sat, 28 Dec 2019 13:13:55 GMT  
		Size: 24.4 MB (24380293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36412f6b2f6e3eabb22af1d89ca68b8d4dff80c6eb05bcc1c1973388e9bc9306`  
		Last Modified: Sat, 28 Dec 2019 13:13:50 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2` - linux; arm variant v5

```console
$ docker pull httpd@sha256:c58de0ddcb5a466c3a15de3cf6dd191131a64c32677c6d0c1fcb57c928a19ccc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.7 MB (56722579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ef4cbc086c5e886ac9ed26b8af3c72d1f7afc1e6ac24c03b79c94facce92bfe`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:57:05 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 05:57:06 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 05:57:08 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 05:57:09 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 05:57:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:57:30 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 05:57:30 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 05:57:33 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 06:02:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 06:02:05 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 06:02:07 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 06:02:11 GMT
EXPOSE 80
# Sat, 28 Dec 2019 06:02:17 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d816054e38989d3ebcb225b5fcc54ad39e7be5939664732283e9e383afeed368`  
		Last Modified: Sat, 28 Dec 2019 06:02:42 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89aecb44adfb6a0eb140304a7a88cc4690b915214fd32bf37b48ef413a3c690e`  
		Last Modified: Sat, 28 Dec 2019 06:02:46 GMT  
		Size: 8.3 MB (8325096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a6eee8ee97aa5e650a4d7a43f29c9b7b81ea11c75555d06ae651cfc8309fbd`  
		Last Modified: Sat, 28 Dec 2019 06:02:49 GMT  
		Size: 23.6 MB (23567390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2325ce68cfb095929fdb719b3b73fc6c1b52760d1470842334938d602e031ef9`  
		Last Modified: Sat, 28 Dec 2019 06:02:42 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2` - linux; arm variant v7

```console
$ docker pull httpd@sha256:28a2183e36c70decb4266ee60488f39c29dee8ad96084e9e75bf9a8d51914bbb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53777666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb940d77142f57935193a488309fba5d03098714c9c4a71344b154db4928ae25`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 12:11:21 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 12:11:22 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 12:11:23 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 12:11:24 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 12:11:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 12:11:44 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 12:11:45 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 12:11:46 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 12:14:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 12:14:59 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 12:15:00 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 12:15:01 GMT
EXPOSE 80
# Sat, 28 Dec 2019 12:15:01 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20c29154beeb7558781d8c78ae337242160edebed61cb9b02449218e7923509`  
		Last Modified: Sat, 28 Dec 2019 12:15:20 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff7b6220a8c45c0bf8ef95ae2cd97b74d72304365dbb1201d7a0efbffebfacc`  
		Last Modified: Sat, 28 Dec 2019 12:15:23 GMT  
		Size: 8.0 MB (7953555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1c28c5c734dc8226ce272eed1b7853d638d9294865551ee06fd39800dd9056`  
		Last Modified: Sat, 28 Dec 2019 12:15:27 GMT  
		Size: 23.1 MB (23124507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb335fdcbd36a9517f416292bb02d659051888e6a5601884d75e79f8423eb09a`  
		Last Modified: Sat, 28 Dec 2019 12:15:19 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2` - linux; arm64 variant v8

```console
$ docker pull httpd@sha256:1fa8b506b23df25b3e2570cd27eb7a88c6d1622e749b7931e9a7f8390d17777b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.2 MB (59181880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58f3666f6461b3ca20529c8ad8b1ef6bfac1baf47d2370b58e260fd2f7bf781a`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:14:03 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 08:14:04 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 08:14:06 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 08:14:06 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 08:14:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:14:25 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 08:14:26 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 08:14:27 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 08:17:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 08:17:31 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 08:17:34 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 08:17:35 GMT
EXPOSE 80
# Sat, 28 Dec 2019 08:17:35 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82403dfe096c9c305f3561111d62d80b364fda9b0e8c444b4c089ad9d9de6696`  
		Last Modified: Sat, 28 Dec 2019 08:18:03 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bbb2355c68c10bb76f3d9ec9909fb56bd7bb4009a028f2f2f8ce168ba9f939`  
		Last Modified: Sat, 28 Dec 2019 08:18:25 GMT  
		Size: 9.0 MB (9040072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0fd60c2f730498b0145c9da328bc47ed55ace03b9752ea520d666b037770c3`  
		Last Modified: Sat, 28 Dec 2019 08:18:10 GMT  
		Size: 24.3 MB (24290630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6239dae9709ab543b813cbea9bc1d736c707306074b447329d403cd2e3a6404`  
		Last Modified: Sat, 28 Dec 2019 08:18:03 GMT  
		Size: 298.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2` - linux; 386

```console
$ docker pull httpd@sha256:940cfd947c03e761c7c1c82113acc775a153a6fc93df05ab7478400a865c57d6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67107611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:988ca54c1d8b0cbaaf3c09b2b82747ca56d7cad0d8e906b7782f118f0fba4793`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 09:20:26 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 09:20:26 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 09:20:28 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 09:20:29 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 09:20:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 09:20:40 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 09:20:40 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 09:20:41 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 09:23:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 09:23:47 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 09:23:48 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 09:23:48 GMT
EXPOSE 80
# Sat, 28 Dec 2019 09:23:48 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b701a2bac4efb85f1ab6fcf6917b04242ba448debab2174e5a3919fc0739471`  
		Last Modified: Sat, 28 Dec 2019 09:24:05 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fe910023bc5d78bfc097a1d54c7f1cdb7b00663ec8019af18dc1e8b17ea968`  
		Last Modified: Sat, 28 Dec 2019 09:24:11 GMT  
		Size: 15.0 MB (15025461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caccb7772535e97c26771b8c0a48b5a9b15f750761dc152a3ca6f9e4beb8bc0f`  
		Last Modified: Sat, 28 Dec 2019 09:24:12 GMT  
		Size: 24.3 MB (24334687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29762e8a543afa52130df42ed7d2e14b3fc4772a26f635bf6d0c58bb67bce131`  
		Last Modified: Sat, 28 Dec 2019 09:24:06 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2` - linux; ppc64le

```console
$ docker pull httpd@sha256:52d7599c192a3d17a07feaec645711f8b10274acdc678996d45ced4b80f0503f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66415921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16fb828297715f1b7a8410601e031a49033155d3971e7fb7fbf9ec294b5696e0`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 09:27:48 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 09:27:52 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 09:27:58 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 09:28:04 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 09:28:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 09:29:07 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 09:29:11 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 09:29:15 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 09:34:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 09:34:45 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 09:34:47 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 09:34:52 GMT
EXPOSE 80
# Sat, 28 Dec 2019 09:34:55 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b7e9b8643623d595015d6f0375fad98e18af2edf3e9efdafaaf46ff2d8e2a2`  
		Last Modified: Sat, 28 Dec 2019 09:35:28 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac2eada050f8bef4b0c3cf94d811126f27b84b7007b23ee140e65aa05c88f82`  
		Last Modified: Sat, 28 Dec 2019 09:35:30 GMT  
		Size: 10.4 MB (10361894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635cc395922662260d099f094461ed10d9157351daa896d0e0856c3f0af1dfb4`  
		Last Modified: Sat, 28 Dec 2019 09:35:32 GMT  
		Size: 25.5 MB (25536025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3659e741869731e9bc61ac358f5e8139da5538784bfd59580158c5f272aaebd7`  
		Last Modified: Sat, 28 Dec 2019 09:35:28 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2` - linux; s390x

```console
$ docker pull httpd@sha256:055480dae600d91cffc45b414a3e2b8892567afd4316775ccc1fb55fef68d434
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58966994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eafe36b5acb400f0ba3a79f743d4a83a182247f1a87cf631a9e661bb3feee502`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:03 GMT
ADD file:eec6c56f8680753860198c3af0d94aabb87018ca30f6f6e346621a6bffe0e4b8 in / 
# Sat, 28 Dec 2019 04:42:04 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:55:59 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 05:55:59 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 05:56:00 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 05:56:00 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 05:56:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:56:07 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 05:56:07 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 05:56:08 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 05:57:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 05:57:47 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 05:57:47 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 05:57:48 GMT
EXPOSE 80
# Sat, 28 Dec 2019 05:57:48 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:f7542f43e95fb32a870ee38d7f0e7bb23267ac8dcf709e3944311b0a30d7a479`  
		Last Modified: Sat, 28 Dec 2019 04:45:08 GMT  
		Size: 25.7 MB (25705315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a920499e61d909a0c5da04045ae14dbdb330ca24260557e89344f9e130ef55`  
		Last Modified: Sat, 28 Dec 2019 05:58:09 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ac5ba88cc154716111293a5580f252b887df15032e079ff7be34b16833ddaf`  
		Last Modified: Sat, 28 Dec 2019 05:58:10 GMT  
		Size: 9.0 MB (9001405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38eeedacfda8dba2f1c461c9cfc3211e094dd0ff34336a692737608470fb96f9`  
		Last Modified: Sat, 28 Dec 2019 05:58:12 GMT  
		Size: 24.3 MB (24259834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85b7ed3eeac346c483c1b3b2a13802483805f652a41c28c28fcb99a3c40e735`  
		Last Modified: Sat, 28 Dec 2019 05:58:09 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `httpd:2.4`

```console
$ docker pull httpd@sha256:769018135ba22d3a7a2b91cb89b8de711562cdf51ad6621b2b9b13e95f3798de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `httpd:2.4` - linux; amd64

```console
$ docker pull httpd@sha256:63dbdd1b6cb325d3afda7774a068ad1c6658490d8d4cd505a4db9d927f9f9afc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.8 MB (61847101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2aa7e16edd855da8827aa0ccf976d1d50f0827c08622c16e0750aa1591717e5`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:08:55 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 13:08:55 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:08:57 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 13:08:57 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 13:09:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:09:05 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 13:09:06 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 13:09:06 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 13:13:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 13:13:36 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 13:13:37 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 13:13:37 GMT
EXPOSE 80
# Sat, 28 Dec 2019 13:13:37 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354e6904d6556707e95c6952df767d7e6447392700fa07d33cd673d28ed80329`  
		Last Modified: Sat, 28 Dec 2019 13:13:50 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27298e4c749a2e37d2842e5200bb388402405c04e2de9fb97a05c868c4df9f7b`  
		Last Modified: Sat, 28 Dec 2019 13:13:53 GMT  
		Size: 10.4 MB (10374093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e27104ba69adc141aa1d84510fd98ae550036abd7a02d4a8881152d18f3aa2`  
		Last Modified: Sat, 28 Dec 2019 13:13:55 GMT  
		Size: 24.4 MB (24380293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36412f6b2f6e3eabb22af1d89ca68b8d4dff80c6eb05bcc1c1973388e9bc9306`  
		Last Modified: Sat, 28 Dec 2019 13:13:50 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4` - linux; arm variant v5

```console
$ docker pull httpd@sha256:c58de0ddcb5a466c3a15de3cf6dd191131a64c32677c6d0c1fcb57c928a19ccc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.7 MB (56722579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ef4cbc086c5e886ac9ed26b8af3c72d1f7afc1e6ac24c03b79c94facce92bfe`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:57:05 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 05:57:06 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 05:57:08 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 05:57:09 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 05:57:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:57:30 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 05:57:30 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 05:57:33 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 06:02:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 06:02:05 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 06:02:07 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 06:02:11 GMT
EXPOSE 80
# Sat, 28 Dec 2019 06:02:17 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d816054e38989d3ebcb225b5fcc54ad39e7be5939664732283e9e383afeed368`  
		Last Modified: Sat, 28 Dec 2019 06:02:42 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89aecb44adfb6a0eb140304a7a88cc4690b915214fd32bf37b48ef413a3c690e`  
		Last Modified: Sat, 28 Dec 2019 06:02:46 GMT  
		Size: 8.3 MB (8325096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a6eee8ee97aa5e650a4d7a43f29c9b7b81ea11c75555d06ae651cfc8309fbd`  
		Last Modified: Sat, 28 Dec 2019 06:02:49 GMT  
		Size: 23.6 MB (23567390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2325ce68cfb095929fdb719b3b73fc6c1b52760d1470842334938d602e031ef9`  
		Last Modified: Sat, 28 Dec 2019 06:02:42 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4` - linux; arm variant v7

```console
$ docker pull httpd@sha256:28a2183e36c70decb4266ee60488f39c29dee8ad96084e9e75bf9a8d51914bbb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53777666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb940d77142f57935193a488309fba5d03098714c9c4a71344b154db4928ae25`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 12:11:21 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 12:11:22 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 12:11:23 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 12:11:24 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 12:11:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 12:11:44 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 12:11:45 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 12:11:46 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 12:14:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 12:14:59 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 12:15:00 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 12:15:01 GMT
EXPOSE 80
# Sat, 28 Dec 2019 12:15:01 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20c29154beeb7558781d8c78ae337242160edebed61cb9b02449218e7923509`  
		Last Modified: Sat, 28 Dec 2019 12:15:20 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff7b6220a8c45c0bf8ef95ae2cd97b74d72304365dbb1201d7a0efbffebfacc`  
		Last Modified: Sat, 28 Dec 2019 12:15:23 GMT  
		Size: 8.0 MB (7953555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1c28c5c734dc8226ce272eed1b7853d638d9294865551ee06fd39800dd9056`  
		Last Modified: Sat, 28 Dec 2019 12:15:27 GMT  
		Size: 23.1 MB (23124507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb335fdcbd36a9517f416292bb02d659051888e6a5601884d75e79f8423eb09a`  
		Last Modified: Sat, 28 Dec 2019 12:15:19 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4` - linux; arm64 variant v8

```console
$ docker pull httpd@sha256:1fa8b506b23df25b3e2570cd27eb7a88c6d1622e749b7931e9a7f8390d17777b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.2 MB (59181880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58f3666f6461b3ca20529c8ad8b1ef6bfac1baf47d2370b58e260fd2f7bf781a`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:14:03 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 08:14:04 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 08:14:06 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 08:14:06 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 08:14:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:14:25 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 08:14:26 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 08:14:27 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 08:17:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 08:17:31 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 08:17:34 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 08:17:35 GMT
EXPOSE 80
# Sat, 28 Dec 2019 08:17:35 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82403dfe096c9c305f3561111d62d80b364fda9b0e8c444b4c089ad9d9de6696`  
		Last Modified: Sat, 28 Dec 2019 08:18:03 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bbb2355c68c10bb76f3d9ec9909fb56bd7bb4009a028f2f2f8ce168ba9f939`  
		Last Modified: Sat, 28 Dec 2019 08:18:25 GMT  
		Size: 9.0 MB (9040072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0fd60c2f730498b0145c9da328bc47ed55ace03b9752ea520d666b037770c3`  
		Last Modified: Sat, 28 Dec 2019 08:18:10 GMT  
		Size: 24.3 MB (24290630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6239dae9709ab543b813cbea9bc1d736c707306074b447329d403cd2e3a6404`  
		Last Modified: Sat, 28 Dec 2019 08:18:03 GMT  
		Size: 298.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4` - linux; 386

```console
$ docker pull httpd@sha256:940cfd947c03e761c7c1c82113acc775a153a6fc93df05ab7478400a865c57d6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67107611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:988ca54c1d8b0cbaaf3c09b2b82747ca56d7cad0d8e906b7782f118f0fba4793`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 09:20:26 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 09:20:26 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 09:20:28 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 09:20:29 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 09:20:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 09:20:40 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 09:20:40 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 09:20:41 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 09:23:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 09:23:47 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 09:23:48 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 09:23:48 GMT
EXPOSE 80
# Sat, 28 Dec 2019 09:23:48 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b701a2bac4efb85f1ab6fcf6917b04242ba448debab2174e5a3919fc0739471`  
		Last Modified: Sat, 28 Dec 2019 09:24:05 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fe910023bc5d78bfc097a1d54c7f1cdb7b00663ec8019af18dc1e8b17ea968`  
		Last Modified: Sat, 28 Dec 2019 09:24:11 GMT  
		Size: 15.0 MB (15025461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caccb7772535e97c26771b8c0a48b5a9b15f750761dc152a3ca6f9e4beb8bc0f`  
		Last Modified: Sat, 28 Dec 2019 09:24:12 GMT  
		Size: 24.3 MB (24334687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29762e8a543afa52130df42ed7d2e14b3fc4772a26f635bf6d0c58bb67bce131`  
		Last Modified: Sat, 28 Dec 2019 09:24:06 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4` - linux; ppc64le

```console
$ docker pull httpd@sha256:52d7599c192a3d17a07feaec645711f8b10274acdc678996d45ced4b80f0503f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66415921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16fb828297715f1b7a8410601e031a49033155d3971e7fb7fbf9ec294b5696e0`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 09:27:48 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 09:27:52 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 09:27:58 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 09:28:04 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 09:28:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 09:29:07 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 09:29:11 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 09:29:15 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 09:34:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 09:34:45 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 09:34:47 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 09:34:52 GMT
EXPOSE 80
# Sat, 28 Dec 2019 09:34:55 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b7e9b8643623d595015d6f0375fad98e18af2edf3e9efdafaaf46ff2d8e2a2`  
		Last Modified: Sat, 28 Dec 2019 09:35:28 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac2eada050f8bef4b0c3cf94d811126f27b84b7007b23ee140e65aa05c88f82`  
		Last Modified: Sat, 28 Dec 2019 09:35:30 GMT  
		Size: 10.4 MB (10361894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635cc395922662260d099f094461ed10d9157351daa896d0e0856c3f0af1dfb4`  
		Last Modified: Sat, 28 Dec 2019 09:35:32 GMT  
		Size: 25.5 MB (25536025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3659e741869731e9bc61ac358f5e8139da5538784bfd59580158c5f272aaebd7`  
		Last Modified: Sat, 28 Dec 2019 09:35:28 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4` - linux; s390x

```console
$ docker pull httpd@sha256:055480dae600d91cffc45b414a3e2b8892567afd4316775ccc1fb55fef68d434
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58966994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eafe36b5acb400f0ba3a79f743d4a83a182247f1a87cf631a9e661bb3feee502`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:03 GMT
ADD file:eec6c56f8680753860198c3af0d94aabb87018ca30f6f6e346621a6bffe0e4b8 in / 
# Sat, 28 Dec 2019 04:42:04 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:55:59 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 05:55:59 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 05:56:00 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 05:56:00 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 05:56:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:56:07 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 05:56:07 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 05:56:08 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 05:57:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 05:57:47 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 05:57:47 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 05:57:48 GMT
EXPOSE 80
# Sat, 28 Dec 2019 05:57:48 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:f7542f43e95fb32a870ee38d7f0e7bb23267ac8dcf709e3944311b0a30d7a479`  
		Last Modified: Sat, 28 Dec 2019 04:45:08 GMT  
		Size: 25.7 MB (25705315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a920499e61d909a0c5da04045ae14dbdb330ca24260557e89344f9e130ef55`  
		Last Modified: Sat, 28 Dec 2019 05:58:09 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ac5ba88cc154716111293a5580f252b887df15032e079ff7be34b16833ddaf`  
		Last Modified: Sat, 28 Dec 2019 05:58:10 GMT  
		Size: 9.0 MB (9001405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38eeedacfda8dba2f1c461c9cfc3211e094dd0ff34336a692737608470fb96f9`  
		Last Modified: Sat, 28 Dec 2019 05:58:12 GMT  
		Size: 24.3 MB (24259834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85b7ed3eeac346c483c1b3b2a13802483805f652a41c28c28fcb99a3c40e735`  
		Last Modified: Sat, 28 Dec 2019 05:58:09 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `httpd:2.4.41`

```console
$ docker pull httpd@sha256:769018135ba22d3a7a2b91cb89b8de711562cdf51ad6621b2b9b13e95f3798de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `httpd:2.4.41` - linux; amd64

```console
$ docker pull httpd@sha256:63dbdd1b6cb325d3afda7774a068ad1c6658490d8d4cd505a4db9d927f9f9afc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.8 MB (61847101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2aa7e16edd855da8827aa0ccf976d1d50f0827c08622c16e0750aa1591717e5`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:08:55 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 13:08:55 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:08:57 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 13:08:57 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 13:09:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:09:05 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 13:09:06 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 13:09:06 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 13:13:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 13:13:36 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 13:13:37 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 13:13:37 GMT
EXPOSE 80
# Sat, 28 Dec 2019 13:13:37 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354e6904d6556707e95c6952df767d7e6447392700fa07d33cd673d28ed80329`  
		Last Modified: Sat, 28 Dec 2019 13:13:50 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27298e4c749a2e37d2842e5200bb388402405c04e2de9fb97a05c868c4df9f7b`  
		Last Modified: Sat, 28 Dec 2019 13:13:53 GMT  
		Size: 10.4 MB (10374093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e27104ba69adc141aa1d84510fd98ae550036abd7a02d4a8881152d18f3aa2`  
		Last Modified: Sat, 28 Dec 2019 13:13:55 GMT  
		Size: 24.4 MB (24380293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36412f6b2f6e3eabb22af1d89ca68b8d4dff80c6eb05bcc1c1973388e9bc9306`  
		Last Modified: Sat, 28 Dec 2019 13:13:50 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4.41` - linux; arm variant v5

```console
$ docker pull httpd@sha256:c58de0ddcb5a466c3a15de3cf6dd191131a64c32677c6d0c1fcb57c928a19ccc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.7 MB (56722579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ef4cbc086c5e886ac9ed26b8af3c72d1f7afc1e6ac24c03b79c94facce92bfe`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:57:05 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 05:57:06 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 05:57:08 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 05:57:09 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 05:57:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:57:30 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 05:57:30 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 05:57:33 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 06:02:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 06:02:05 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 06:02:07 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 06:02:11 GMT
EXPOSE 80
# Sat, 28 Dec 2019 06:02:17 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d816054e38989d3ebcb225b5fcc54ad39e7be5939664732283e9e383afeed368`  
		Last Modified: Sat, 28 Dec 2019 06:02:42 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89aecb44adfb6a0eb140304a7a88cc4690b915214fd32bf37b48ef413a3c690e`  
		Last Modified: Sat, 28 Dec 2019 06:02:46 GMT  
		Size: 8.3 MB (8325096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a6eee8ee97aa5e650a4d7a43f29c9b7b81ea11c75555d06ae651cfc8309fbd`  
		Last Modified: Sat, 28 Dec 2019 06:02:49 GMT  
		Size: 23.6 MB (23567390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2325ce68cfb095929fdb719b3b73fc6c1b52760d1470842334938d602e031ef9`  
		Last Modified: Sat, 28 Dec 2019 06:02:42 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4.41` - linux; arm variant v7

```console
$ docker pull httpd@sha256:28a2183e36c70decb4266ee60488f39c29dee8ad96084e9e75bf9a8d51914bbb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53777666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb940d77142f57935193a488309fba5d03098714c9c4a71344b154db4928ae25`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 12:11:21 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 12:11:22 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 12:11:23 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 12:11:24 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 12:11:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 12:11:44 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 12:11:45 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 12:11:46 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 12:14:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 12:14:59 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 12:15:00 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 12:15:01 GMT
EXPOSE 80
# Sat, 28 Dec 2019 12:15:01 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20c29154beeb7558781d8c78ae337242160edebed61cb9b02449218e7923509`  
		Last Modified: Sat, 28 Dec 2019 12:15:20 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff7b6220a8c45c0bf8ef95ae2cd97b74d72304365dbb1201d7a0efbffebfacc`  
		Last Modified: Sat, 28 Dec 2019 12:15:23 GMT  
		Size: 8.0 MB (7953555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1c28c5c734dc8226ce272eed1b7853d638d9294865551ee06fd39800dd9056`  
		Last Modified: Sat, 28 Dec 2019 12:15:27 GMT  
		Size: 23.1 MB (23124507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb335fdcbd36a9517f416292bb02d659051888e6a5601884d75e79f8423eb09a`  
		Last Modified: Sat, 28 Dec 2019 12:15:19 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4.41` - linux; arm64 variant v8

```console
$ docker pull httpd@sha256:1fa8b506b23df25b3e2570cd27eb7a88c6d1622e749b7931e9a7f8390d17777b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.2 MB (59181880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58f3666f6461b3ca20529c8ad8b1ef6bfac1baf47d2370b58e260fd2f7bf781a`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:14:03 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 08:14:04 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 08:14:06 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 08:14:06 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 08:14:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:14:25 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 08:14:26 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 08:14:27 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 08:17:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 08:17:31 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 08:17:34 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 08:17:35 GMT
EXPOSE 80
# Sat, 28 Dec 2019 08:17:35 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82403dfe096c9c305f3561111d62d80b364fda9b0e8c444b4c089ad9d9de6696`  
		Last Modified: Sat, 28 Dec 2019 08:18:03 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bbb2355c68c10bb76f3d9ec9909fb56bd7bb4009a028f2f2f8ce168ba9f939`  
		Last Modified: Sat, 28 Dec 2019 08:18:25 GMT  
		Size: 9.0 MB (9040072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0fd60c2f730498b0145c9da328bc47ed55ace03b9752ea520d666b037770c3`  
		Last Modified: Sat, 28 Dec 2019 08:18:10 GMT  
		Size: 24.3 MB (24290630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6239dae9709ab543b813cbea9bc1d736c707306074b447329d403cd2e3a6404`  
		Last Modified: Sat, 28 Dec 2019 08:18:03 GMT  
		Size: 298.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4.41` - linux; 386

```console
$ docker pull httpd@sha256:940cfd947c03e761c7c1c82113acc775a153a6fc93df05ab7478400a865c57d6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67107611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:988ca54c1d8b0cbaaf3c09b2b82747ca56d7cad0d8e906b7782f118f0fba4793`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 09:20:26 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 09:20:26 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 09:20:28 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 09:20:29 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 09:20:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 09:20:40 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 09:20:40 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 09:20:41 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 09:23:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 09:23:47 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 09:23:48 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 09:23:48 GMT
EXPOSE 80
# Sat, 28 Dec 2019 09:23:48 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b701a2bac4efb85f1ab6fcf6917b04242ba448debab2174e5a3919fc0739471`  
		Last Modified: Sat, 28 Dec 2019 09:24:05 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fe910023bc5d78bfc097a1d54c7f1cdb7b00663ec8019af18dc1e8b17ea968`  
		Last Modified: Sat, 28 Dec 2019 09:24:11 GMT  
		Size: 15.0 MB (15025461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caccb7772535e97c26771b8c0a48b5a9b15f750761dc152a3ca6f9e4beb8bc0f`  
		Last Modified: Sat, 28 Dec 2019 09:24:12 GMT  
		Size: 24.3 MB (24334687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29762e8a543afa52130df42ed7d2e14b3fc4772a26f635bf6d0c58bb67bce131`  
		Last Modified: Sat, 28 Dec 2019 09:24:06 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4.41` - linux; ppc64le

```console
$ docker pull httpd@sha256:52d7599c192a3d17a07feaec645711f8b10274acdc678996d45ced4b80f0503f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66415921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16fb828297715f1b7a8410601e031a49033155d3971e7fb7fbf9ec294b5696e0`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 09:27:48 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 09:27:52 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 09:27:58 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 09:28:04 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 09:28:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 09:29:07 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 09:29:11 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 09:29:15 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 09:34:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 09:34:45 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 09:34:47 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 09:34:52 GMT
EXPOSE 80
# Sat, 28 Dec 2019 09:34:55 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b7e9b8643623d595015d6f0375fad98e18af2edf3e9efdafaaf46ff2d8e2a2`  
		Last Modified: Sat, 28 Dec 2019 09:35:28 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac2eada050f8bef4b0c3cf94d811126f27b84b7007b23ee140e65aa05c88f82`  
		Last Modified: Sat, 28 Dec 2019 09:35:30 GMT  
		Size: 10.4 MB (10361894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635cc395922662260d099f094461ed10d9157351daa896d0e0856c3f0af1dfb4`  
		Last Modified: Sat, 28 Dec 2019 09:35:32 GMT  
		Size: 25.5 MB (25536025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3659e741869731e9bc61ac358f5e8139da5538784bfd59580158c5f272aaebd7`  
		Last Modified: Sat, 28 Dec 2019 09:35:28 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4.41` - linux; s390x

```console
$ docker pull httpd@sha256:055480dae600d91cffc45b414a3e2b8892567afd4316775ccc1fb55fef68d434
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58966994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eafe36b5acb400f0ba3a79f743d4a83a182247f1a87cf631a9e661bb3feee502`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:03 GMT
ADD file:eec6c56f8680753860198c3af0d94aabb87018ca30f6f6e346621a6bffe0e4b8 in / 
# Sat, 28 Dec 2019 04:42:04 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:55:59 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 05:55:59 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 05:56:00 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 05:56:00 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 05:56:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:56:07 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 05:56:07 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 05:56:08 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 05:57:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 05:57:47 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 05:57:47 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 05:57:48 GMT
EXPOSE 80
# Sat, 28 Dec 2019 05:57:48 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:f7542f43e95fb32a870ee38d7f0e7bb23267ac8dcf709e3944311b0a30d7a479`  
		Last Modified: Sat, 28 Dec 2019 04:45:08 GMT  
		Size: 25.7 MB (25705315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a920499e61d909a0c5da04045ae14dbdb330ca24260557e89344f9e130ef55`  
		Last Modified: Sat, 28 Dec 2019 05:58:09 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ac5ba88cc154716111293a5580f252b887df15032e079ff7be34b16833ddaf`  
		Last Modified: Sat, 28 Dec 2019 05:58:10 GMT  
		Size: 9.0 MB (9001405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38eeedacfda8dba2f1c461c9cfc3211e094dd0ff34336a692737608470fb96f9`  
		Last Modified: Sat, 28 Dec 2019 05:58:12 GMT  
		Size: 24.3 MB (24259834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85b7ed3eeac346c483c1b3b2a13802483805f652a41c28c28fcb99a3c40e735`  
		Last Modified: Sat, 28 Dec 2019 05:58:09 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `httpd:2.4.41-alpine`

```console
$ docker pull httpd@sha256:ca20eca5ae5c1be31bdf99d700d86d9164edd71bcf519325bde67ed04aa1008f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `httpd:2.4.41-alpine` - linux; amd64

```console
$ docker pull httpd@sha256:cd9cb9f0148b56a4d8f4f58be6a59d9c23d4c8d6c88f4a53736e6c7ca66b742c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33651339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb171b88ec9231dba1a54af4790c8f38164b64158f3dff912bf4e600da22d02b`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:15:35 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:15:35 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 03:15:35 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:15:36 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 03:15:36 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 03:15:36 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 03:15:36 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 03:15:36 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 03:16:43 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 03:16:44 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 03:16:44 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:16:44 GMT
EXPOSE 80
# Sat, 18 Jan 2020 03:16:44 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f37b2be62f65b2f4c9a37ef7a9618353a3bfd484e46ad980e29eb27e89f1a19`  
		Last Modified: Sat, 18 Jan 2020 03:16:53 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badbb502951ee75b0845321b1063fa4be257d4cdbbcbb85fcb940b1d90e7665c`  
		Last Modified: Sat, 18 Jan 2020 03:16:53 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27b80e2bf04a3e33d4cf55c059bbd789f7e2a7a2380ef77846f185de403a68e`  
		Last Modified: Sat, 18 Jan 2020 03:17:00 GMT  
		Size: 30.8 MB (30846712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c005fed9a91da450f731f737580e003c4576dc248cf9833eca0255edf14d669`  
		Last Modified: Sat, 18 Jan 2020 03:16:53 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4.41-alpine` - linux; arm variant v6

```console
$ docker pull httpd@sha256:dad9f89b6fc9523d9809b58d2d0861e2921214cfa2c1ccbdcb767907cf4aded3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31821671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3047850d5d7b669437f108a3285846133e463758428a30b417da375efc845a`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:33:05 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 04:33:13 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 04:33:17 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:33:32 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 04:33:40 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 04:33:48 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 04:33:55 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 04:34:00 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 04:36:16 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 04:36:25 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 04:36:27 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:36:30 GMT
EXPOSE 80
# Sat, 18 Jan 2020 04:36:33 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f44c7801479402905523f05b467e26bda1f5e31c3b5c034496c98893f42f28`  
		Last Modified: Sat, 18 Jan 2020 04:36:51 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1da429945cfb889882c17e6b1ad86987ffbd8592cb0bb0bd1da3a9848f97b6`  
		Last Modified: Sat, 18 Jan 2020 04:36:51 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e035b74a1a145d9560404f0fbbfaecde59dc4fc4c1384d92f1ace9e99e7ebb41`  
		Last Modified: Sat, 18 Jan 2020 04:37:05 GMT  
		Size: 29.2 MB (29202377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0a84f76323b0dd74fcc03696485418fa33f857da1d4b466dee82ddbaa55f9c`  
		Last Modified: Sat, 18 Jan 2020 04:36:51 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4.41-alpine` - linux; arm variant v7

```console
$ docker pull httpd@sha256:7088e15ec84966dc53101a436bb6a63df75221d7a378438043c3011a0f81d81e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.1 MB (30122528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660a04821efc588b6ae4c146b4588c4bbb830304b3a2f4d8ecaed3d8d750c010`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:18:53 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:18:53 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 03:18:54 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:18:55 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 03:18:56 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 03:18:56 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 03:18:57 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 03:18:58 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 03:20:26 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 03:20:29 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 03:20:29 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:20:30 GMT
EXPOSE 80
# Sat, 18 Jan 2020 03:20:31 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db77d63f7e40d78e49be7b325f8a7dadb95ad1d8c952b681d90238ff135e424`  
		Last Modified: Sat, 18 Jan 2020 03:20:58 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a265a84129f512deb898ef4982986c7d002b3819719b18c5ebe075c2791a8b81`  
		Last Modified: Sat, 18 Jan 2020 03:20:58 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92a8951a9028faaef49965b4c1f66a7bb5bd645cedb47a5bab30ea9fe58c45b`  
		Last Modified: Sat, 18 Jan 2020 03:21:10 GMT  
		Size: 27.7 MB (27701242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f0658a7d634286ee0cda85c38e68dd3fcb5c253a3610b2f8da68f6a41fd8cd`  
		Last Modified: Sat, 18 Jan 2020 03:20:58 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4.41-alpine` - linux; arm64 variant v8

```console
$ docker pull httpd@sha256:b61173cdc116aca7595994db674183a75b2aa1dd796845bfa243e0bc9f1f293c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33667987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82f3294b668e7c076744e7e6ef050b3f93d57bfd988865a71069cc9804a66604`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:18:36 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 02:18:37 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 02:18:38 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 02:18:45 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 02:18:46 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 02:18:47 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 02:18:49 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 02:18:50 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 02:21:13 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 02:21:16 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 02:21:19 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:21:22 GMT
EXPOSE 80
# Sat, 18 Jan 2020 02:21:23 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505e4a20cddd77b884ff165d3964b29b04ced7b22bd1e208a513cd3d7f65b534`  
		Last Modified: Sat, 18 Jan 2020 02:21:43 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc656df2bc24b9c4da86a0be2ae3d7b7273fef55ee8f31d54dee437b2fa084e`  
		Last Modified: Sat, 18 Jan 2020 02:21:43 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1564c14ddd9099ce823c109171b2a144c78226207af705d3900534a49fe43750`  
		Last Modified: Sat, 18 Jan 2020 02:21:56 GMT  
		Size: 30.9 MB (30943178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f456d21cc47a318fb66c2295d9f81f920e11ca5e9bbb678dd1753b3a92bd82`  
		Last Modified: Sat, 18 Jan 2020 02:21:43 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4.41-alpine` - linux; 386

```console
$ docker pull httpd@sha256:390c237ff9840cff81b84238928525a318b1f62fe7c1a68be6543dece4683b6b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33912028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4329464e7a90e73f3fccdb94967c01d7612880580527335eeeed5ffcf455a4c`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:38:52 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 05:38:52 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 05:38:52 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 05:38:53 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 05:38:53 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 05:38:53 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 05:38:53 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 05:38:54 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 05:40:22 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 05:40:23 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 05:40:23 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:40:23 GMT
EXPOSE 80
# Sat, 18 Jan 2020 05:40:23 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a761a2b418774d9b5bfcbf6750764b5518435473c1b45ca4b139ac20a144ef`  
		Last Modified: Sat, 18 Jan 2020 05:40:42 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e364dd9a97cfe443d751d06d05b564409a37a0b42515008a88b401c197ae8346`  
		Last Modified: Sat, 18 Jan 2020 05:40:42 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4793a1e08d3efece0988402ed9b312fda3a2b43c229a67b4883865e65a4f3e`  
		Last Modified: Sat, 18 Jan 2020 05:40:52 GMT  
		Size: 31.1 MB (31103798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466eae814c69fedf2dafa31ee27ee9ef6ab4d237ec6465c2aa4b3823a7415811`  
		Last Modified: Sat, 18 Jan 2020 05:40:42 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4.41-alpine` - linux; ppc64le

```console
$ docker pull httpd@sha256:d09438aa37bd9dfaebc33647923bc7b06e390fa5fdc57ba3d6eaf7043864abf6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (34975441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2666008465df189d5f0391b7cc126ca57d2638bea74a8493ab122e35e2c90c`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:40:43 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 04:40:46 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 04:40:48 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:40:52 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 04:40:54 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 04:40:55 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 04:40:57 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 04:40:58 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 04:42:10 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 04:42:14 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 04:42:15 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:17 GMT
EXPOSE 80
# Sat, 18 Jan 2020 04:42:19 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e2a7320ac6bafb4c08a0595128e78db8b95ca01343cf6303be01ada8695865`  
		Last Modified: Sat, 18 Jan 2020 04:42:44 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776d399fd9ba64dd6be01659a4b99ece3866bdce6cf831f927c3653b35220662`  
		Last Modified: Sat, 18 Jan 2020 04:42:44 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b400ba6b97de646f2ac04d7e47d734b4a94242deb397503e5f596d1077dd61`  
		Last Modified: Sat, 18 Jan 2020 04:42:53 GMT  
		Size: 32.2 MB (32151579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4ee9eb88205cb694498bd38cdb9319b66fc1a1bc8d957e0699ff0228e9b37d`  
		Last Modified: Sat, 18 Jan 2020 04:42:44 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4.41-alpine` - linux; s390x

```console
$ docker pull httpd@sha256:9420a4d46a516a150cf083cf38b76497be8c78718750d03a51b54195dbe3a2a4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34349767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f066242c489f32d7866070652128ec3e536943e3d6d9373190631e6956c214ff`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:42:48 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:42:48 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 03:42:48 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:42:49 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 03:42:49 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 03:42:49 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 03:42:49 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 03:42:50 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 03:43:33 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 03:43:33 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 03:43:34 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:43:34 GMT
EXPOSE 80
# Sat, 18 Jan 2020 03:43:34 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4626fee82182479dffd32f8191f0957b7f7d489712b7c0a811a509f3775fec`  
		Last Modified: Sat, 18 Jan 2020 03:43:47 GMT  
		Size: 1.2 KB (1235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41825abff682046b75f93ff2bbe83617c82aa59457ce0ad817ee68151305ad70`  
		Last Modified: Sat, 18 Jan 2020 03:43:47 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727fb05f8bebb3c418fd788a1f858b48d067a3331b32f42331cd99fc83a5a980`  
		Last Modified: Sat, 18 Jan 2020 03:43:53 GMT  
		Size: 31.8 MB (31766062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4343c6cdc248ce08d22e55e0582220ae27db51883bbee6022a6b98ec81222b7`  
		Last Modified: Sat, 18 Jan 2020 03:43:47 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `httpd:2.4-alpine`

```console
$ docker pull httpd@sha256:ca20eca5ae5c1be31bdf99d700d86d9164edd71bcf519325bde67ed04aa1008f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `httpd:2.4-alpine` - linux; amd64

```console
$ docker pull httpd@sha256:cd9cb9f0148b56a4d8f4f58be6a59d9c23d4c8d6c88f4a53736e6c7ca66b742c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33651339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb171b88ec9231dba1a54af4790c8f38164b64158f3dff912bf4e600da22d02b`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:15:35 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:15:35 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 03:15:35 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:15:36 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 03:15:36 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 03:15:36 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 03:15:36 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 03:15:36 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 03:16:43 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 03:16:44 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 03:16:44 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:16:44 GMT
EXPOSE 80
# Sat, 18 Jan 2020 03:16:44 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f37b2be62f65b2f4c9a37ef7a9618353a3bfd484e46ad980e29eb27e89f1a19`  
		Last Modified: Sat, 18 Jan 2020 03:16:53 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badbb502951ee75b0845321b1063fa4be257d4cdbbcbb85fcb940b1d90e7665c`  
		Last Modified: Sat, 18 Jan 2020 03:16:53 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27b80e2bf04a3e33d4cf55c059bbd789f7e2a7a2380ef77846f185de403a68e`  
		Last Modified: Sat, 18 Jan 2020 03:17:00 GMT  
		Size: 30.8 MB (30846712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c005fed9a91da450f731f737580e003c4576dc248cf9833eca0255edf14d669`  
		Last Modified: Sat, 18 Jan 2020 03:16:53 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4-alpine` - linux; arm variant v6

```console
$ docker pull httpd@sha256:dad9f89b6fc9523d9809b58d2d0861e2921214cfa2c1ccbdcb767907cf4aded3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31821671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3047850d5d7b669437f108a3285846133e463758428a30b417da375efc845a`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:33:05 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 04:33:13 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 04:33:17 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:33:32 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 04:33:40 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 04:33:48 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 04:33:55 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 04:34:00 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 04:36:16 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 04:36:25 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 04:36:27 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:36:30 GMT
EXPOSE 80
# Sat, 18 Jan 2020 04:36:33 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f44c7801479402905523f05b467e26bda1f5e31c3b5c034496c98893f42f28`  
		Last Modified: Sat, 18 Jan 2020 04:36:51 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1da429945cfb889882c17e6b1ad86987ffbd8592cb0bb0bd1da3a9848f97b6`  
		Last Modified: Sat, 18 Jan 2020 04:36:51 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e035b74a1a145d9560404f0fbbfaecde59dc4fc4c1384d92f1ace9e99e7ebb41`  
		Last Modified: Sat, 18 Jan 2020 04:37:05 GMT  
		Size: 29.2 MB (29202377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0a84f76323b0dd74fcc03696485418fa33f857da1d4b466dee82ddbaa55f9c`  
		Last Modified: Sat, 18 Jan 2020 04:36:51 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4-alpine` - linux; arm variant v7

```console
$ docker pull httpd@sha256:7088e15ec84966dc53101a436bb6a63df75221d7a378438043c3011a0f81d81e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.1 MB (30122528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660a04821efc588b6ae4c146b4588c4bbb830304b3a2f4d8ecaed3d8d750c010`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:18:53 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:18:53 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 03:18:54 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:18:55 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 03:18:56 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 03:18:56 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 03:18:57 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 03:18:58 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 03:20:26 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 03:20:29 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 03:20:29 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:20:30 GMT
EXPOSE 80
# Sat, 18 Jan 2020 03:20:31 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db77d63f7e40d78e49be7b325f8a7dadb95ad1d8c952b681d90238ff135e424`  
		Last Modified: Sat, 18 Jan 2020 03:20:58 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a265a84129f512deb898ef4982986c7d002b3819719b18c5ebe075c2791a8b81`  
		Last Modified: Sat, 18 Jan 2020 03:20:58 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92a8951a9028faaef49965b4c1f66a7bb5bd645cedb47a5bab30ea9fe58c45b`  
		Last Modified: Sat, 18 Jan 2020 03:21:10 GMT  
		Size: 27.7 MB (27701242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f0658a7d634286ee0cda85c38e68dd3fcb5c253a3610b2f8da68f6a41fd8cd`  
		Last Modified: Sat, 18 Jan 2020 03:20:58 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4-alpine` - linux; arm64 variant v8

```console
$ docker pull httpd@sha256:b61173cdc116aca7595994db674183a75b2aa1dd796845bfa243e0bc9f1f293c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33667987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82f3294b668e7c076744e7e6ef050b3f93d57bfd988865a71069cc9804a66604`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:18:36 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 02:18:37 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 02:18:38 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 02:18:45 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 02:18:46 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 02:18:47 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 02:18:49 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 02:18:50 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 02:21:13 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 02:21:16 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 02:21:19 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:21:22 GMT
EXPOSE 80
# Sat, 18 Jan 2020 02:21:23 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505e4a20cddd77b884ff165d3964b29b04ced7b22bd1e208a513cd3d7f65b534`  
		Last Modified: Sat, 18 Jan 2020 02:21:43 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc656df2bc24b9c4da86a0be2ae3d7b7273fef55ee8f31d54dee437b2fa084e`  
		Last Modified: Sat, 18 Jan 2020 02:21:43 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1564c14ddd9099ce823c109171b2a144c78226207af705d3900534a49fe43750`  
		Last Modified: Sat, 18 Jan 2020 02:21:56 GMT  
		Size: 30.9 MB (30943178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f456d21cc47a318fb66c2295d9f81f920e11ca5e9bbb678dd1753b3a92bd82`  
		Last Modified: Sat, 18 Jan 2020 02:21:43 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4-alpine` - linux; 386

```console
$ docker pull httpd@sha256:390c237ff9840cff81b84238928525a318b1f62fe7c1a68be6543dece4683b6b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33912028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4329464e7a90e73f3fccdb94967c01d7612880580527335eeeed5ffcf455a4c`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:38:52 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 05:38:52 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 05:38:52 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 05:38:53 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 05:38:53 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 05:38:53 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 05:38:53 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 05:38:54 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 05:40:22 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 05:40:23 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 05:40:23 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:40:23 GMT
EXPOSE 80
# Sat, 18 Jan 2020 05:40:23 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a761a2b418774d9b5bfcbf6750764b5518435473c1b45ca4b139ac20a144ef`  
		Last Modified: Sat, 18 Jan 2020 05:40:42 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e364dd9a97cfe443d751d06d05b564409a37a0b42515008a88b401c197ae8346`  
		Last Modified: Sat, 18 Jan 2020 05:40:42 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4793a1e08d3efece0988402ed9b312fda3a2b43c229a67b4883865e65a4f3e`  
		Last Modified: Sat, 18 Jan 2020 05:40:52 GMT  
		Size: 31.1 MB (31103798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466eae814c69fedf2dafa31ee27ee9ef6ab4d237ec6465c2aa4b3823a7415811`  
		Last Modified: Sat, 18 Jan 2020 05:40:42 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4-alpine` - linux; ppc64le

```console
$ docker pull httpd@sha256:d09438aa37bd9dfaebc33647923bc7b06e390fa5fdc57ba3d6eaf7043864abf6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (34975441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2666008465df189d5f0391b7cc126ca57d2638bea74a8493ab122e35e2c90c`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:40:43 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 04:40:46 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 04:40:48 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:40:52 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 04:40:54 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 04:40:55 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 04:40:57 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 04:40:58 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 04:42:10 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 04:42:14 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 04:42:15 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:17 GMT
EXPOSE 80
# Sat, 18 Jan 2020 04:42:19 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e2a7320ac6bafb4c08a0595128e78db8b95ca01343cf6303be01ada8695865`  
		Last Modified: Sat, 18 Jan 2020 04:42:44 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776d399fd9ba64dd6be01659a4b99ece3866bdce6cf831f927c3653b35220662`  
		Last Modified: Sat, 18 Jan 2020 04:42:44 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b400ba6b97de646f2ac04d7e47d734b4a94242deb397503e5f596d1077dd61`  
		Last Modified: Sat, 18 Jan 2020 04:42:53 GMT  
		Size: 32.2 MB (32151579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4ee9eb88205cb694498bd38cdb9319b66fc1a1bc8d957e0699ff0228e9b37d`  
		Last Modified: Sat, 18 Jan 2020 04:42:44 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2.4-alpine` - linux; s390x

```console
$ docker pull httpd@sha256:9420a4d46a516a150cf083cf38b76497be8c78718750d03a51b54195dbe3a2a4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34349767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f066242c489f32d7866070652128ec3e536943e3d6d9373190631e6956c214ff`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:42:48 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:42:48 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 03:42:48 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:42:49 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 03:42:49 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 03:42:49 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 03:42:49 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 03:42:50 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 03:43:33 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 03:43:33 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 03:43:34 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:43:34 GMT
EXPOSE 80
# Sat, 18 Jan 2020 03:43:34 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4626fee82182479dffd32f8191f0957b7f7d489712b7c0a811a509f3775fec`  
		Last Modified: Sat, 18 Jan 2020 03:43:47 GMT  
		Size: 1.2 KB (1235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41825abff682046b75f93ff2bbe83617c82aa59457ce0ad817ee68151305ad70`  
		Last Modified: Sat, 18 Jan 2020 03:43:47 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727fb05f8bebb3c418fd788a1f858b48d067a3331b32f42331cd99fc83a5a980`  
		Last Modified: Sat, 18 Jan 2020 03:43:53 GMT  
		Size: 31.8 MB (31766062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4343c6cdc248ce08d22e55e0582220ae27db51883bbee6022a6b98ec81222b7`  
		Last Modified: Sat, 18 Jan 2020 03:43:47 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `httpd:2-alpine`

```console
$ docker pull httpd@sha256:ca20eca5ae5c1be31bdf99d700d86d9164edd71bcf519325bde67ed04aa1008f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `httpd:2-alpine` - linux; amd64

```console
$ docker pull httpd@sha256:cd9cb9f0148b56a4d8f4f58be6a59d9c23d4c8d6c88f4a53736e6c7ca66b742c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33651339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb171b88ec9231dba1a54af4790c8f38164b64158f3dff912bf4e600da22d02b`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:15:35 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:15:35 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 03:15:35 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:15:36 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 03:15:36 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 03:15:36 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 03:15:36 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 03:15:36 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 03:16:43 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 03:16:44 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 03:16:44 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:16:44 GMT
EXPOSE 80
# Sat, 18 Jan 2020 03:16:44 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f37b2be62f65b2f4c9a37ef7a9618353a3bfd484e46ad980e29eb27e89f1a19`  
		Last Modified: Sat, 18 Jan 2020 03:16:53 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badbb502951ee75b0845321b1063fa4be257d4cdbbcbb85fcb940b1d90e7665c`  
		Last Modified: Sat, 18 Jan 2020 03:16:53 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27b80e2bf04a3e33d4cf55c059bbd789f7e2a7a2380ef77846f185de403a68e`  
		Last Modified: Sat, 18 Jan 2020 03:17:00 GMT  
		Size: 30.8 MB (30846712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c005fed9a91da450f731f737580e003c4576dc248cf9833eca0255edf14d669`  
		Last Modified: Sat, 18 Jan 2020 03:16:53 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; arm variant v6

```console
$ docker pull httpd@sha256:dad9f89b6fc9523d9809b58d2d0861e2921214cfa2c1ccbdcb767907cf4aded3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31821671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3047850d5d7b669437f108a3285846133e463758428a30b417da375efc845a`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:33:05 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 04:33:13 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 04:33:17 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:33:32 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 04:33:40 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 04:33:48 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 04:33:55 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 04:34:00 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 04:36:16 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 04:36:25 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 04:36:27 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:36:30 GMT
EXPOSE 80
# Sat, 18 Jan 2020 04:36:33 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f44c7801479402905523f05b467e26bda1f5e31c3b5c034496c98893f42f28`  
		Last Modified: Sat, 18 Jan 2020 04:36:51 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1da429945cfb889882c17e6b1ad86987ffbd8592cb0bb0bd1da3a9848f97b6`  
		Last Modified: Sat, 18 Jan 2020 04:36:51 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e035b74a1a145d9560404f0fbbfaecde59dc4fc4c1384d92f1ace9e99e7ebb41`  
		Last Modified: Sat, 18 Jan 2020 04:37:05 GMT  
		Size: 29.2 MB (29202377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0a84f76323b0dd74fcc03696485418fa33f857da1d4b466dee82ddbaa55f9c`  
		Last Modified: Sat, 18 Jan 2020 04:36:51 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; arm variant v7

```console
$ docker pull httpd@sha256:7088e15ec84966dc53101a436bb6a63df75221d7a378438043c3011a0f81d81e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.1 MB (30122528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660a04821efc588b6ae4c146b4588c4bbb830304b3a2f4d8ecaed3d8d750c010`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:18:53 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:18:53 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 03:18:54 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:18:55 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 03:18:56 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 03:18:56 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 03:18:57 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 03:18:58 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 03:20:26 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 03:20:29 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 03:20:29 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:20:30 GMT
EXPOSE 80
# Sat, 18 Jan 2020 03:20:31 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db77d63f7e40d78e49be7b325f8a7dadb95ad1d8c952b681d90238ff135e424`  
		Last Modified: Sat, 18 Jan 2020 03:20:58 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a265a84129f512deb898ef4982986c7d002b3819719b18c5ebe075c2791a8b81`  
		Last Modified: Sat, 18 Jan 2020 03:20:58 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92a8951a9028faaef49965b4c1f66a7bb5bd645cedb47a5bab30ea9fe58c45b`  
		Last Modified: Sat, 18 Jan 2020 03:21:10 GMT  
		Size: 27.7 MB (27701242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f0658a7d634286ee0cda85c38e68dd3fcb5c253a3610b2f8da68f6a41fd8cd`  
		Last Modified: Sat, 18 Jan 2020 03:20:58 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; arm64 variant v8

```console
$ docker pull httpd@sha256:b61173cdc116aca7595994db674183a75b2aa1dd796845bfa243e0bc9f1f293c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33667987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82f3294b668e7c076744e7e6ef050b3f93d57bfd988865a71069cc9804a66604`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:18:36 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 02:18:37 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 02:18:38 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 02:18:45 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 02:18:46 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 02:18:47 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 02:18:49 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 02:18:50 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 02:21:13 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 02:21:16 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 02:21:19 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:21:22 GMT
EXPOSE 80
# Sat, 18 Jan 2020 02:21:23 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505e4a20cddd77b884ff165d3964b29b04ced7b22bd1e208a513cd3d7f65b534`  
		Last Modified: Sat, 18 Jan 2020 02:21:43 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc656df2bc24b9c4da86a0be2ae3d7b7273fef55ee8f31d54dee437b2fa084e`  
		Last Modified: Sat, 18 Jan 2020 02:21:43 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1564c14ddd9099ce823c109171b2a144c78226207af705d3900534a49fe43750`  
		Last Modified: Sat, 18 Jan 2020 02:21:56 GMT  
		Size: 30.9 MB (30943178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f456d21cc47a318fb66c2295d9f81f920e11ca5e9bbb678dd1753b3a92bd82`  
		Last Modified: Sat, 18 Jan 2020 02:21:43 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; 386

```console
$ docker pull httpd@sha256:390c237ff9840cff81b84238928525a318b1f62fe7c1a68be6543dece4683b6b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33912028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4329464e7a90e73f3fccdb94967c01d7612880580527335eeeed5ffcf455a4c`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:38:52 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 05:38:52 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 05:38:52 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 05:38:53 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 05:38:53 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 05:38:53 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 05:38:53 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 05:38:54 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 05:40:22 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 05:40:23 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 05:40:23 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:40:23 GMT
EXPOSE 80
# Sat, 18 Jan 2020 05:40:23 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a761a2b418774d9b5bfcbf6750764b5518435473c1b45ca4b139ac20a144ef`  
		Last Modified: Sat, 18 Jan 2020 05:40:42 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e364dd9a97cfe443d751d06d05b564409a37a0b42515008a88b401c197ae8346`  
		Last Modified: Sat, 18 Jan 2020 05:40:42 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4793a1e08d3efece0988402ed9b312fda3a2b43c229a67b4883865e65a4f3e`  
		Last Modified: Sat, 18 Jan 2020 05:40:52 GMT  
		Size: 31.1 MB (31103798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466eae814c69fedf2dafa31ee27ee9ef6ab4d237ec6465c2aa4b3823a7415811`  
		Last Modified: Sat, 18 Jan 2020 05:40:42 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; ppc64le

```console
$ docker pull httpd@sha256:d09438aa37bd9dfaebc33647923bc7b06e390fa5fdc57ba3d6eaf7043864abf6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (34975441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2666008465df189d5f0391b7cc126ca57d2638bea74a8493ab122e35e2c90c`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:40:43 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 04:40:46 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 04:40:48 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:40:52 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 04:40:54 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 04:40:55 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 04:40:57 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 04:40:58 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 04:42:10 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 04:42:14 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 04:42:15 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:17 GMT
EXPOSE 80
# Sat, 18 Jan 2020 04:42:19 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e2a7320ac6bafb4c08a0595128e78db8b95ca01343cf6303be01ada8695865`  
		Last Modified: Sat, 18 Jan 2020 04:42:44 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776d399fd9ba64dd6be01659a4b99ece3866bdce6cf831f927c3653b35220662`  
		Last Modified: Sat, 18 Jan 2020 04:42:44 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b400ba6b97de646f2ac04d7e47d734b4a94242deb397503e5f596d1077dd61`  
		Last Modified: Sat, 18 Jan 2020 04:42:53 GMT  
		Size: 32.2 MB (32151579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4ee9eb88205cb694498bd38cdb9319b66fc1a1bc8d957e0699ff0228e9b37d`  
		Last Modified: Sat, 18 Jan 2020 04:42:44 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; s390x

```console
$ docker pull httpd@sha256:9420a4d46a516a150cf083cf38b76497be8c78718750d03a51b54195dbe3a2a4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34349767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f066242c489f32d7866070652128ec3e536943e3d6d9373190631e6956c214ff`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:42:48 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:42:48 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 03:42:48 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:42:49 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 03:42:49 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 03:42:49 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 03:42:49 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 03:42:50 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 03:43:33 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 03:43:33 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 03:43:34 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:43:34 GMT
EXPOSE 80
# Sat, 18 Jan 2020 03:43:34 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4626fee82182479dffd32f8191f0957b7f7d489712b7c0a811a509f3775fec`  
		Last Modified: Sat, 18 Jan 2020 03:43:47 GMT  
		Size: 1.2 KB (1235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41825abff682046b75f93ff2bbe83617c82aa59457ce0ad817ee68151305ad70`  
		Last Modified: Sat, 18 Jan 2020 03:43:47 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727fb05f8bebb3c418fd788a1f858b48d067a3331b32f42331cd99fc83a5a980`  
		Last Modified: Sat, 18 Jan 2020 03:43:53 GMT  
		Size: 31.8 MB (31766062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4343c6cdc248ce08d22e55e0582220ae27db51883bbee6022a6b98ec81222b7`  
		Last Modified: Sat, 18 Jan 2020 03:43:47 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `httpd:alpine`

```console
$ docker pull httpd@sha256:ca20eca5ae5c1be31bdf99d700d86d9164edd71bcf519325bde67ed04aa1008f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `httpd:alpine` - linux; amd64

```console
$ docker pull httpd@sha256:cd9cb9f0148b56a4d8f4f58be6a59d9c23d4c8d6c88f4a53736e6c7ca66b742c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33651339 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cb171b88ec9231dba1a54af4790c8f38164b64158f3dff912bf4e600da22d02b`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:19:37 GMT
ADD file:e69d441d729412d24675dcd33e04580885df99981cec43de8c9b24015313ff8e in / 
# Sat, 18 Jan 2020 01:19:37 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:15:35 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:15:35 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 03:15:35 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:15:36 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 03:15:36 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 03:15:36 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 03:15:36 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 03:15:36 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 03:16:43 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 03:16:44 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 03:16:44 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:16:44 GMT
EXPOSE 80
# Sat, 18 Jan 2020 03:16:44 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:c9b1b535fdd91a9855fb7f82348177e5f019329a58c53c47272962dd60f71fc9`  
		Last Modified: Fri, 17 Jan 2020 08:04:01 GMT  
		Size: 2.8 MB (2802957 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f37b2be62f65b2f4c9a37ef7a9618353a3bfd484e46ad980e29eb27e89f1a19`  
		Last Modified: Sat, 18 Jan 2020 03:16:53 GMT  
		Size: 1.2 KB (1231 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:badbb502951ee75b0845321b1063fa4be257d4cdbbcbb85fcb940b1d90e7665c`  
		Last Modified: Sat, 18 Jan 2020 03:16:53 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27b80e2bf04a3e33d4cf55c059bbd789f7e2a7a2380ef77846f185de403a68e`  
		Last Modified: Sat, 18 Jan 2020 03:17:00 GMT  
		Size: 30.8 MB (30846712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c005fed9a91da450f731f737580e003c4576dc248cf9833eca0255edf14d669`  
		Last Modified: Sat, 18 Jan 2020 03:16:53 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:alpine` - linux; arm variant v6

```console
$ docker pull httpd@sha256:dad9f89b6fc9523d9809b58d2d0861e2921214cfa2c1ccbdcb767907cf4aded3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **31.8 MB (31821671 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:af3047850d5d7b669437f108a3285846133e463758428a30b417da375efc845a`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:53:16 GMT
ADD file:a1906f14a4e217a498b550f86a3d17c9012c02a6df0668043b63848c8fa44b9b in / 
# Sat, 18 Jan 2020 01:53:17 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:33:05 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 04:33:13 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 04:33:17 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:33:32 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 04:33:40 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 04:33:48 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 04:33:55 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 04:34:00 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 04:36:16 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 04:36:25 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 04:36:27 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:36:30 GMT
EXPOSE 80
# Sat, 18 Jan 2020 04:36:33 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:832e07764099264ef96e50a1e5e41c52d6b0809bd054e29508a6878aa59d156d`  
		Last Modified: Sat, 18 Jan 2020 01:53:52 GMT  
		Size: 2.6 MB (2617562 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3f44c7801479402905523f05b467e26bda1f5e31c3b5c034496c98893f42f28`  
		Last Modified: Sat, 18 Jan 2020 04:36:51 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1da429945cfb889882c17e6b1ad86987ffbd8592cb0bb0bd1da3a9848f97b6`  
		Last Modified: Sat, 18 Jan 2020 04:36:51 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e035b74a1a145d9560404f0fbbfaecde59dc4fc4c1384d92f1ace9e99e7ebb41`  
		Last Modified: Sat, 18 Jan 2020 04:37:05 GMT  
		Size: 29.2 MB (29202377 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a0a84f76323b0dd74fcc03696485418fa33f857da1d4b466dee82ddbaa55f9c`  
		Last Modified: Sat, 18 Jan 2020 04:36:51 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:alpine` - linux; arm variant v7

```console
$ docker pull httpd@sha256:7088e15ec84966dc53101a436bb6a63df75221d7a378438043c3011a0f81d81e
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **30.1 MB (30122528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:660a04821efc588b6ae4c146b4588c4bbb830304b3a2f4d8ecaed3d8d750c010`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 02:03:19 GMT
ADD file:4c815f4461ff3b8d481f43d84eb2548cb1adbb3015d370cab86dd7f4d3d94279 in / 
# Sat, 18 Jan 2020 02:03:22 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:18:53 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:18:53 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 03:18:54 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:18:55 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 03:18:56 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 03:18:56 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 03:18:57 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 03:18:58 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 03:20:26 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 03:20:29 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 03:20:29 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:20:30 GMT
EXPOSE 80
# Sat, 18 Jan 2020 03:20:31 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:3a2c5e3c37b2e3d749405512ef3793aa45a2f5c11615d9e9efa80179262cdf27`  
		Last Modified: Sat, 18 Jan 2020 02:04:05 GMT  
		Size: 2.4 MB (2419554 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1db77d63f7e40d78e49be7b325f8a7dadb95ad1d8c952b681d90238ff135e424`  
		Last Modified: Sat, 18 Jan 2020 03:20:58 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a265a84129f512deb898ef4982986c7d002b3819719b18c5ebe075c2791a8b81`  
		Last Modified: Sat, 18 Jan 2020 03:20:58 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b92a8951a9028faaef49965b4c1f66a7bb5bd645cedb47a5bab30ea9fe58c45b`  
		Last Modified: Sat, 18 Jan 2020 03:21:10 GMT  
		Size: 27.7 MB (27701242 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64f0658a7d634286ee0cda85c38e68dd3fcb5c253a3610b2f8da68f6a41fd8cd`  
		Last Modified: Sat, 18 Jan 2020 03:20:58 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:alpine` - linux; arm64 variant v8

```console
$ docker pull httpd@sha256:b61173cdc116aca7595994db674183a75b2aa1dd796845bfa243e0bc9f1f293c
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.7 MB (33667987 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:82f3294b668e7c076744e7e6ef050b3f93d57bfd988865a71069cc9804a66604`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:39:43 GMT
ADD file:4109fa86dd80850e84c689ff9e6a3243e30ab1bbcc00c765969b3011bfbb43e1 in / 
# Sat, 18 Jan 2020 01:39:43 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 02:18:36 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 02:18:37 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 02:18:38 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 02:18:45 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 02:18:46 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 02:18:47 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 02:18:49 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 02:18:50 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 02:21:13 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 02:21:16 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 02:21:19 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 02:21:22 GMT
EXPOSE 80
# Sat, 18 Jan 2020 02:21:23 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:8fa90b21c985a6fcfff966bdfbde81cdd088de0aa8af38110057f6ac408f4408`  
		Last Modified: Sat, 18 Jan 2020 01:40:23 GMT  
		Size: 2.7 MB (2723075 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:505e4a20cddd77b884ff165d3964b29b04ced7b22bd1e208a513cd3d7f65b534`  
		Last Modified: Sat, 18 Jan 2020 02:21:43 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bc656df2bc24b9c4da86a0be2ae3d7b7273fef55ee8f31d54dee437b2fa084e`  
		Last Modified: Sat, 18 Jan 2020 02:21:43 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1564c14ddd9099ce823c109171b2a144c78226207af705d3900534a49fe43750`  
		Last Modified: Sat, 18 Jan 2020 02:21:56 GMT  
		Size: 30.9 MB (30943178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f456d21cc47a318fb66c2295d9f81f920e11ca5e9bbb678dd1753b3a92bd82`  
		Last Modified: Sat, 18 Jan 2020 02:21:43 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:alpine` - linux; 386

```console
$ docker pull httpd@sha256:390c237ff9840cff81b84238928525a318b1f62fe7c1a68be6543dece4683b6b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **33.9 MB (33912028 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b4329464e7a90e73f3fccdb94967c01d7612880580527335eeeed5ffcf455a4c`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:38:44 GMT
ADD file:381b617b92fe699ad4ef4f30e0d9599f89e43e252883348c420ebe2a0cccbd63 in / 
# Sat, 18 Jan 2020 01:38:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 05:38:52 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 05:38:52 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 05:38:52 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 05:38:53 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 05:38:53 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 05:38:53 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 05:38:53 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 05:38:54 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 05:40:22 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 05:40:23 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 05:40:23 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 05:40:23 GMT
EXPOSE 80
# Sat, 18 Jan 2020 05:40:23 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:f024b1263dc58db07a458b73ae1a2dca02ca55bef1ccd1fa3fd50656551fadf2`  
		Last Modified: Sat, 18 Jan 2020 01:39:18 GMT  
		Size: 2.8 MB (2806560 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21a761a2b418774d9b5bfcbf6750764b5518435473c1b45ca4b139ac20a144ef`  
		Last Modified: Sat, 18 Jan 2020 05:40:42 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e364dd9a97cfe443d751d06d05b564409a37a0b42515008a88b401c197ae8346`  
		Last Modified: Sat, 18 Jan 2020 05:40:42 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f4793a1e08d3efece0988402ed9b312fda3a2b43c229a67b4883865e65a4f3e`  
		Last Modified: Sat, 18 Jan 2020 05:40:52 GMT  
		Size: 31.1 MB (31103798 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:466eae814c69fedf2dafa31ee27ee9ef6ab4d237ec6465c2aa4b3823a7415811`  
		Last Modified: Sat, 18 Jan 2020 05:40:42 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:alpine` - linux; ppc64le

```console
$ docker pull httpd@sha256:d09438aa37bd9dfaebc33647923bc7b06e390fa5fdc57ba3d6eaf7043864abf6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.0 MB (34975441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a2666008465df189d5f0391b7cc126ca57d2638bea74a8493ab122e35e2c90c`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 02:20:41 GMT
ADD file:32ddb3d5255071cca51573ceee2464dd5a87c8d1cce514ae965b6e824d9ef24b in / 
# Sat, 18 Jan 2020 02:20:45 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 04:40:43 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 04:40:46 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 04:40:48 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 04:40:52 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 04:40:54 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 04:40:55 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 04:40:57 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 04:40:58 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 04:42:10 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 04:42:14 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 04:42:15 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 04:42:17 GMT
EXPOSE 80
# Sat, 18 Jan 2020 04:42:19 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:cd95c8a93e39dcaa0634a65d5b86a88bcd5c3092adb1f96504a7030faa165123`  
		Last Modified: Sat, 18 Jan 2020 02:21:25 GMT  
		Size: 2.8 MB (2822125 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68e2a7320ac6bafb4c08a0595128e78db8b95ca01343cf6303be01ada8695865`  
		Last Modified: Sat, 18 Jan 2020 04:42:44 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:776d399fd9ba64dd6be01659a4b99ece3866bdce6cf831f927c3653b35220662`  
		Last Modified: Sat, 18 Jan 2020 04:42:44 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18b400ba6b97de646f2ac04d7e47d734b4a94242deb397503e5f596d1077dd61`  
		Last Modified: Sat, 18 Jan 2020 04:42:53 GMT  
		Size: 32.2 MB (32151579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f4ee9eb88205cb694498bd38cdb9319b66fc1a1bc8d957e0699ff0228e9b37d`  
		Last Modified: Sat, 18 Jan 2020 04:42:44 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:alpine` - linux; s390x

```console
$ docker pull httpd@sha256:9420a4d46a516a150cf083cf38b76497be8c78718750d03a51b54195dbe3a2a4
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.3 MB (34349767 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f066242c489f32d7866070652128ec3e536943e3d6d9373190631e6956c214ff`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 18 Jan 2020 01:41:33 GMT
ADD file:a6f8b7d4ba199527053ef1ac710b5e318135cb6903cb9ad6fae4fe42e6ad0bf7 in / 
# Sat, 18 Jan 2020 01:41:33 GMT
CMD ["/bin/sh"]
# Sat, 18 Jan 2020 03:42:48 GMT
RUN set -x 	&& addgroup -g 82 -S www-data 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 18 Jan 2020 03:42:48 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 18 Jan 2020 03:42:48 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 18 Jan 2020 03:42:49 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 18 Jan 2020 03:42:49 GMT
WORKDIR /usr/local/apache2
# Sat, 18 Jan 2020 03:42:49 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 18 Jan 2020 03:42:49 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 18 Jan 2020 03:42:50 GMT
ENV HTTPD_PATCHES=
# Sat, 18 Jan 2020 03:43:33 GMT
RUN set -eux; 		runDeps=' 		apr-dev 		apr-util-dbm_db 		apr-util-dev 		apr-util-ldap 		perl 	'; 	apk add --no-cache --virtual .build-deps 		$runDeps 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		runDeps="$runDeps $( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-rundeps $runDeps; 	apk del --no-network .build-deps; 		httpd -v
# Sat, 18 Jan 2020 03:43:33 GMT
STOPSIGNAL SIGWINCH
# Sat, 18 Jan 2020 03:43:34 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 18 Jan 2020 03:43:34 GMT
EXPOSE 80
# Sat, 18 Jan 2020 03:43:34 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:176bad61a3a435da03ec603d2bd8f7a69286d92f21f447b17f21f0bc4e085bde`  
		Last Modified: Sat, 18 Jan 2020 01:41:59 GMT  
		Size: 2.6 MB (2582031 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d4626fee82182479dffd32f8191f0957b7f7d489712b7c0a811a509f3775fec`  
		Last Modified: Sat, 18 Jan 2020 03:43:47 GMT  
		Size: 1.2 KB (1235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:41825abff682046b75f93ff2bbe83617c82aa59457ce0ad817ee68151305ad70`  
		Last Modified: Sat, 18 Jan 2020 03:43:47 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:727fb05f8bebb3c418fd788a1f858b48d067a3331b32f42331cd99fc83a5a980`  
		Last Modified: Sat, 18 Jan 2020 03:43:53 GMT  
		Size: 31.8 MB (31766062 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4343c6cdc248ce08d22e55e0582220ae27db51883bbee6022a6b98ec81222b7`  
		Last Modified: Sat, 18 Jan 2020 03:43:47 GMT  
		Size: 293.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `httpd:latest`

```console
$ docker pull httpd@sha256:769018135ba22d3a7a2b91cb89b8de711562cdf51ad6621b2b9b13e95f3798de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v5
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `httpd:latest` - linux; amd64

```console
$ docker pull httpd@sha256:63dbdd1b6cb325d3afda7774a068ad1c6658490d8d4cd505a4db9d927f9f9afc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.8 MB (61847101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c2aa7e16edd855da8827aa0ccf976d1d50f0827c08622c16e0750aa1591717e5`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:21:22 GMT
ADD file:04caaf303199c81ff1a94e2e39d5096f9d02b73294b82758e5bc6e23aff94272 in / 
# Sat, 28 Dec 2019 04:21:23 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 13:08:55 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 13:08:55 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 13:08:57 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 13:08:57 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 13:09:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 13:09:05 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 13:09:06 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 13:09:06 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 13:13:36 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 13:13:36 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 13:13:37 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 13:13:37 GMT
EXPOSE 80
# Sat, 28 Dec 2019 13:13:37 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:8ec398bc03560e0fa56440e96da307cdf0b1ad153f459b52bca53ae7ddb8236d`  
		Last Modified: Sat, 28 Dec 2019 04:25:53 GMT  
		Size: 27.1 MB (27092274 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:354e6904d6556707e95c6952df767d7e6447392700fa07d33cd673d28ed80329`  
		Last Modified: Sat, 28 Dec 2019 13:13:50 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27298e4c749a2e37d2842e5200bb388402405c04e2de9fb97a05c868c4df9f7b`  
		Last Modified: Sat, 28 Dec 2019 13:13:53 GMT  
		Size: 10.4 MB (10374093 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10e27104ba69adc141aa1d84510fd98ae550036abd7a02d4a8881152d18f3aa2`  
		Last Modified: Sat, 28 Dec 2019 13:13:55 GMT  
		Size: 24.4 MB (24380293 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36412f6b2f6e3eabb22af1d89ca68b8d4dff80c6eb05bcc1c1973388e9bc9306`  
		Last Modified: Sat, 28 Dec 2019 13:13:50 GMT  
		Size: 295.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:latest` - linux; arm variant v5

```console
$ docker pull httpd@sha256:c58de0ddcb5a466c3a15de3cf6dd191131a64c32677c6d0c1fcb57c928a19ccc
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **56.7 MB (56722579 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ef4cbc086c5e886ac9ed26b8af3c72d1f7afc1e6ac24c03b79c94facce92bfe`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:49:50 GMT
ADD file:5d34c769f80c3fdbb04048f4336cf212164934607a642144ef557faef5896192 in / 
# Sat, 28 Dec 2019 04:49:51 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:57:05 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 05:57:06 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 05:57:08 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 05:57:09 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 05:57:29 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:57:30 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 05:57:30 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 05:57:33 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 06:02:01 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 06:02:05 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 06:02:07 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 06:02:11 GMT
EXPOSE 80
# Sat, 28 Dec 2019 06:02:17 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:153ccec980772b5fc4c786af0b26bba09f0a2d95d9755400febf9a79aa4220c8`  
		Last Modified: Sat, 28 Dec 2019 04:56:28 GMT  
		Size: 24.8 MB (24829618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d816054e38989d3ebcb225b5fcc54ad39e7be5939664732283e9e383afeed368`  
		Last Modified: Sat, 28 Dec 2019 06:02:42 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:89aecb44adfb6a0eb140304a7a88cc4690b915214fd32bf37b48ef413a3c690e`  
		Last Modified: Sat, 28 Dec 2019 06:02:46 GMT  
		Size: 8.3 MB (8325096 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83a6eee8ee97aa5e650a4d7a43f29c9b7b81ea11c75555d06ae651cfc8309fbd`  
		Last Modified: Sat, 28 Dec 2019 06:02:49 GMT  
		Size: 23.6 MB (23567390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2325ce68cfb095929fdb719b3b73fc6c1b52760d1470842334938d602e031ef9`  
		Last Modified: Sat, 28 Dec 2019 06:02:42 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:latest` - linux; arm variant v7

```console
$ docker pull httpd@sha256:28a2183e36c70decb4266ee60488f39c29dee8ad96084e9e75bf9a8d51914bbb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.8 MB (53777666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fb940d77142f57935193a488309fba5d03098714c9c4a71344b154db4928ae25`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:59:06 GMT
ADD file:d252ae1c97d5c80e71e64a51cc4d137a901e0e6cdc4aec29faa917fa9bcf3242 in / 
# Sat, 28 Dec 2019 04:59:08 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 12:11:21 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 12:11:22 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 12:11:23 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 12:11:24 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 12:11:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 12:11:44 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 12:11:45 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 12:11:46 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 12:14:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 12:14:59 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 12:15:00 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 12:15:01 GMT
EXPOSE 80
# Sat, 28 Dec 2019 12:15:01 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:c4f8e1e649d2e7938fbe832f157cfb695319ee625a8bc06c619219a87d550949`  
		Last Modified: Sat, 28 Dec 2019 05:07:32 GMT  
		Size: 22.7 MB (22699129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d20c29154beeb7558781d8c78ae337242160edebed61cb9b02449218e7923509`  
		Last Modified: Sat, 28 Dec 2019 12:15:20 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dff7b6220a8c45c0bf8ef95ae2cd97b74d72304365dbb1201d7a0efbffebfacc`  
		Last Modified: Sat, 28 Dec 2019 12:15:23 GMT  
		Size: 8.0 MB (7953555 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bd1c28c5c734dc8226ce272eed1b7853d638d9294865551ee06fd39800dd9056`  
		Last Modified: Sat, 28 Dec 2019 12:15:27 GMT  
		Size: 23.1 MB (23124507 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb335fdcbd36a9517f416292bb02d659051888e6a5601884d75e79f8423eb09a`  
		Last Modified: Sat, 28 Dec 2019 12:15:19 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:latest` - linux; arm64 variant v8

```console
$ docker pull httpd@sha256:1fa8b506b23df25b3e2570cd27eb7a88c6d1622e749b7931e9a7f8390d17777b
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.2 MB (59181880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58f3666f6461b3ca20529c8ad8b1ef6bfac1baf47d2370b58e260fd2f7bf781a`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:41:08 GMT
ADD file:b45fd612576b682e93ab91addbc4387a6609ace4bc092e5b615323964bba33c3 in / 
# Sat, 28 Dec 2019 04:41:11 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 08:14:03 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 08:14:04 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 08:14:06 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 08:14:06 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 08:14:24 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 08:14:25 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 08:14:26 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 08:14:27 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 08:17:30 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 08:17:31 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 08:17:34 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 08:17:35 GMT
EXPOSE 80
# Sat, 28 Dec 2019 08:17:35 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:fb62b7c746da1f79992359282f2d8b7f93da8c48dc138ec6b2a36130efd42635`  
		Last Modified: Sat, 28 Dec 2019 04:46:58 GMT  
		Size: 25.9 MB (25850702 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82403dfe096c9c305f3561111d62d80b364fda9b0e8c444b4c089ad9d9de6696`  
		Last Modified: Sat, 28 Dec 2019 08:18:03 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6bbb2355c68c10bb76f3d9ec9909fb56bd7bb4009a028f2f2f8ce168ba9f939`  
		Last Modified: Sat, 28 Dec 2019 08:18:25 GMT  
		Size: 9.0 MB (9040072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b0fd60c2f730498b0145c9da328bc47ed55ace03b9752ea520d666b037770c3`  
		Last Modified: Sat, 28 Dec 2019 08:18:10 GMT  
		Size: 24.3 MB (24290630 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6239dae9709ab543b813cbea9bc1d736c707306074b447329d403cd2e3a6404`  
		Last Modified: Sat, 28 Dec 2019 08:18:03 GMT  
		Size: 298.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:latest` - linux; 386

```console
$ docker pull httpd@sha256:940cfd947c03e761c7c1c82113acc775a153a6fc93df05ab7478400a865c57d6
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.1 MB (67107611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:988ca54c1d8b0cbaaf3c09b2b82747ca56d7cad0d8e906b7782f118f0fba4793`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:39:35 GMT
ADD file:447f0758c9f5653f03d964e54a38c18f24cf4c43e05fc38e7a76aebd6d6bafa8 in / 
# Sat, 28 Dec 2019 04:39:35 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 09:20:26 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 09:20:26 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 09:20:28 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 09:20:29 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 09:20:39 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 09:20:40 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 09:20:40 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 09:20:41 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 09:23:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 09:23:47 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 09:23:48 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 09:23:48 GMT
EXPOSE 80
# Sat, 28 Dec 2019 09:23:48 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:5536417213b9f46f2118943c1151912954d6077afe03a32e68521774cc358095`  
		Last Modified: Sat, 28 Dec 2019 04:44:24 GMT  
		Size: 27.7 MB (27747020 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b701a2bac4efb85f1ab6fcf6917b04242ba448debab2174e5a3919fc0739471`  
		Last Modified: Sat, 28 Dec 2019 09:24:05 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49fe910023bc5d78bfc097a1d54c7f1cdb7b00663ec8019af18dc1e8b17ea968`  
		Last Modified: Sat, 28 Dec 2019 09:24:11 GMT  
		Size: 15.0 MB (15025461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:caccb7772535e97c26771b8c0a48b5a9b15f750761dc152a3ca6f9e4beb8bc0f`  
		Last Modified: Sat, 28 Dec 2019 09:24:12 GMT  
		Size: 24.3 MB (24334687 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29762e8a543afa52130df42ed7d2e14b3fc4772a26f635bf6d0c58bb67bce131`  
		Last Modified: Sat, 28 Dec 2019 09:24:06 GMT  
		Size: 296.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:latest` - linux; ppc64le

```console
$ docker pull httpd@sha256:52d7599c192a3d17a07feaec645711f8b10274acdc678996d45ced4b80f0503f
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.4 MB (66415921 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16fb828297715f1b7a8410601e031a49033155d3971e7fb7fbf9ec294b5696e0`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:20:39 GMT
ADD file:abec4f3d6a54bb0725560d826d07e99da3d6b582433c6dd95605626c67d7c2d6 in / 
# Sat, 28 Dec 2019 04:20:43 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 09:27:48 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 09:27:52 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 09:27:58 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 09:28:04 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 09:28:58 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 09:29:07 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 09:29:11 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 09:29:15 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 09:34:38 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 09:34:45 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 09:34:47 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 09:34:52 GMT
EXPOSE 80
# Sat, 28 Dec 2019 09:34:55 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:37e6f4d596ea5c3cc92914bd95508a4192c8834c4edaff414734885929b07800`  
		Last Modified: Sat, 28 Dec 2019 04:28:05 GMT  
		Size: 30.5 MB (30517529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73b7e9b8643623d595015d6f0375fad98e18af2edf3e9efdafaaf46ff2d8e2a2`  
		Last Modified: Sat, 28 Dec 2019 09:35:28 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac2eada050f8bef4b0c3cf94d811126f27b84b7007b23ee140e65aa05c88f82`  
		Last Modified: Sat, 28 Dec 2019 09:35:30 GMT  
		Size: 10.4 MB (10361894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635cc395922662260d099f094461ed10d9157351daa896d0e0856c3f0af1dfb4`  
		Last Modified: Sat, 28 Dec 2019 09:35:32 GMT  
		Size: 25.5 MB (25536025 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3659e741869731e9bc61ac358f5e8139da5538784bfd59580158c5f272aaebd7`  
		Last Modified: Sat, 28 Dec 2019 09:35:28 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:latest` - linux; s390x

```console
$ docker pull httpd@sha256:055480dae600d91cffc45b414a3e2b8892567afd4316775ccc1fb55fef68d434
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **59.0 MB (58966994 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eafe36b5acb400f0ba3a79f743d4a83a182247f1a87cf631a9e661bb3feee502`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 28 Dec 2019 04:42:03 GMT
ADD file:eec6c56f8680753860198c3af0d94aabb87018ca30f6f6e346621a6bffe0e4b8 in / 
# Sat, 28 Dec 2019 04:42:04 GMT
CMD ["bash"]
# Sat, 28 Dec 2019 05:55:59 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 28 Dec 2019 05:55:59 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 28 Dec 2019 05:56:00 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 28 Dec 2019 05:56:00 GMT
WORKDIR /usr/local/apache2
# Sat, 28 Dec 2019 05:56:07 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libapr1-dev 		libaprutil1-dev 		libaprutil1-ldap 	; 	rm -rf /var/lib/apt/lists/*
# Sat, 28 Dec 2019 05:56:07 GMT
ENV HTTPD_VERSION=2.4.41
# Sat, 28 Dec 2019 05:56:07 GMT
ENV HTTPD_SHA256=133d48298fe5315ae9366a0ec66282fa4040efa5d566174481077ade7d18ea40
# Sat, 28 Dec 2019 05:56:08 GMT
ENV HTTPD_PATCHES=
# Sat, 28 Dec 2019 05:57:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		bzip2 		ca-certificates 		dirmngr 		dpkg-dev 		gcc 		gnupg 		libbrotli-dev 		libcurl4-openssl-dev 		libjansson-dev 		liblua5.2-dev 		libnghttp2-dev 		libpcre3-dev 		libssl-dev 		libxml2-dev 		make 		wget 		zlib1g-dev 	; 	rm -r /var/lib/apt/lists/*; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		B9E8213AEFB861AF35A41F2C995E35221AD84DFF 	; do 		gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	CFLAGS="$(dpkg-buildflags --get CFLAGS)"; 	CPPFLAGS="$(dpkg-buildflags --get CPPFLAGS)"; 	LDFLAGS="$(dpkg-buildflags --get LDFLAGS)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 		--enable-pie 		CFLAGS="-pipe $CFLAGS" 		CPPFLAGS="$CPPFLAGS" 		LDFLAGS="-Wl,--as-needed $LDFLAGS" 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { print $(NF-1) }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		httpd -v
# Sat, 28 Dec 2019 05:57:47 GMT
STOPSIGNAL SIGWINCH
# Sat, 28 Dec 2019 05:57:47 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Sat, 28 Dec 2019 05:57:48 GMT
EXPOSE 80
# Sat, 28 Dec 2019 05:57:48 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:f7542f43e95fb32a870ee38d7f0e7bb23267ac8dcf709e3944311b0a30d7a479`  
		Last Modified: Sat, 28 Dec 2019 04:45:08 GMT  
		Size: 25.7 MB (25705315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53a920499e61d909a0c5da04045ae14dbdb330ca24260557e89344f9e130ef55`  
		Last Modified: Sat, 28 Dec 2019 05:58:09 GMT  
		Size: 146.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54ac5ba88cc154716111293a5580f252b887df15032e079ff7be34b16833ddaf`  
		Last Modified: Sat, 28 Dec 2019 05:58:10 GMT  
		Size: 9.0 MB (9001405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38eeedacfda8dba2f1c461c9cfc3211e094dd0ff34336a692737608470fb96f9`  
		Last Modified: Sat, 28 Dec 2019 05:58:12 GMT  
		Size: 24.3 MB (24259834 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e85b7ed3eeac346c483c1b3b2a13802483805f652a41c28c28fcb99a3c40e735`  
		Last Modified: Sat, 28 Dec 2019 05:58:09 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
