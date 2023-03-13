## `httpd:2-alpine`

```console
$ docker pull httpd@sha256:b63c5961bebaf9f66ed059c323bc82553fd22d72fb897baae3a0981b1089bb63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 7
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `httpd:2-alpine` - linux; amd64

```console
$ docker pull httpd@sha256:e9068055aad2e2ecf0d3cada9d017dc3770f1a7521cf3d6a3aae2e587873f3b2
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17422437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1e551f571d95f76d27811305e99b4674eca3e5bd35015c122554d5eb15538b0`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:43:06 GMT
RUN set -x 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 09:43:06 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 11 Feb 2023 09:43:06 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 09:43:06 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 11 Feb 2023 09:43:06 GMT
WORKDIR /usr/local/apache2
# Sat, 11 Feb 2023 09:43:08 GMT
RUN set -eux; 	apk add --no-cache 		apr 		apr-util 		apr-util-ldap 		ca-certificates 		perl 	;
# Tue, 07 Mar 2023 20:24:25 GMT
ENV HTTPD_VERSION=2.4.56
# Tue, 07 Mar 2023 20:24:25 GMT
ENV HTTPD_SHA256=d8d45f1398ba84edd05bb33ca7593ac2989b17cb9c7a0cafe5442d41afdb2d7c
# Tue, 07 Mar 2023 20:24:25 GMT
ENV HTTPD_PATCHES=
# Tue, 07 Mar 2023 20:25:39 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		apr-dev 		apr-util-dev 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://downloads.apache.org/ 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		DE29FB3971E71543FD2DC049508EAEC5302DA568 		13155B0E9E634F42BF6C163FDDBA64BA2C312D2F 		8B39757B1D8A994DF2433ED58B3A601F08C975E5 		31EE1A81B8D066548156D37B7D6DBFD1F08E012A 		A10208FEC3152DD7C0C9B59B361522D782AB7BD1 		3DE024AFDA7A4B15CB6C14410F81AA8AB0D5F771 		EB138C6AF0FC691001B16D93344A844D751D7F27 		CBA5A7C21EC143314C41393E5B968010E04F9A89 		3C016F2B764621BB549C66B516A96495E2226795 		937FB3994A242BA9BF49E93021454AF0CC8B0F7E 		EAD1359A4C0F2D37472AAF28F55DF0293A4E7AC9 		4C1EADADB4EF5007579C919C6635B6C0DE885DD3 		01E475360FCCF1D0F24B9D145D414AE1E005C9CB 		92CCEF0AA7DD46AC3A0F498BCA6939748103A37E 		D395C7573A68B9796D38C258153FA0CD75A67692 		FA39B617B61493FD283503E7EED1EA392261D073 		984FB3350C1D5C7A3282255BB31B213D208F5064 		FE7A49DAA875E890B4167F76CCB2EB46E76CF6D0 		39F6691A0ECF0C50E8BB849CF78875F642721F00 		29A2BA848177B73878277FA475CAA2A3F39B3750 		120A8667241AEDD4A78B46104C042818311A3DE5 		453510BDA6C5855624E009236D0BC73A40581837 		0DE5C55C6BF3B2352DABB89E13249B4FEC88A0BF 		7CDBED100806552182F98844E8E7E00B4DAA1988 		A8BA9617EF3BCCAC3B29B869EDB105896F9522D8 		3E6AC004854F3A7F03566B592FF06894E55B0D0E 		5B5181C2C0AB13E59DA3F7A3EC582EB639FF092C 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		65B2D44FE74BD5E3DE3AC3F082781DE46D5954FA 		8935926745E1CE7E3ED748F6EC99EE267EB5F61A 		E3480043595621FE56105F112AB12A7ADC55C003 		93525CFCF6FDFFB3FD9700DD5A4B10AE43B56A27 		C55AB7B9139EB2263CD1AABC19B033D1760C227B 		26F51EF9A82F4ACB43F1903ED377C9E7D1944C66 	; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*User)\s+daemon\s*$!\1 www-data!g' 		-e 's!^(\s*Group)\s+daemon\s*$!\1 www-data!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 	grep -E '^\s*User www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 	grep -E '^\s*Group www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 		deps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-so-deps $deps; 	apk del --no-network .build-deps; 		httpd -v
# Tue, 07 Mar 2023 20:25:40 GMT
STOPSIGNAL SIGWINCH
# Tue, 07 Mar 2023 20:25:40 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Tue, 07 Mar 2023 20:25:40 GMT
EXPOSE 80
# Tue, 07 Mar 2023 20:25:40 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7233f37399d2b38e180ff4511d403623006bd630acdd3ef8a2277737c0f881`  
		Last Modified: Sat, 11 Feb 2023 09:44:47 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a49cb9b71696ca3e3d3725dab652a4d5fb940aafadee799cf381592eb238ad4`  
		Last Modified: Sat, 11 Feb 2023 09:44:47 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:56e6e368b425382c3fc100b05c371fd91cbddc9f4dc53f72b5e971ad11311130`  
		Last Modified: Sat, 11 Feb 2023 09:44:50 GMT  
		Size: 9.9 MB (9870938 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c7c2b83a7a78f9600451f577eaf9f190d03b69f95a5b664e2ce1987b98a6ae1`  
		Last Modified: Tue, 07 Mar 2023 20:26:31 GMT  
		Size: 4.2 MB (4175313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d30d21842c5be3dcf737a02d5132bb6244e1ce6131c5baccad5becb9ea064e0d`  
		Last Modified: Tue, 07 Mar 2023 20:26:30 GMT  
		Size: 298.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; arm variant v6

```console
$ docker pull httpd@sha256:a44e4691e3b158707ed23a96636e70b1fc1e06138f3461893099cde6b524601c
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.6 MB (16574880 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b619921d53f1d54e0a40743299aaa81a0bbd3092654412df4e8c98a38be86bbb`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Mon, 13 Mar 2023 16:12:44 GMT
ADD file:d825d9aef59df0df23c0140a490998407ee0a62a051699b5c050aef7cb03f042 in / 
# Mon, 13 Mar 2023 16:12:44 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 16:45:39 GMT
RUN set -x 	&& adduser -u 82 -D -S -G www-data www-data
# Mon, 13 Mar 2023 16:45:39 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Mon, 13 Mar 2023 16:45:39 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 13 Mar 2023 16:45:39 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Mon, 13 Mar 2023 16:45:40 GMT
WORKDIR /usr/local/apache2
# Mon, 13 Mar 2023 16:45:43 GMT
RUN set -eux; 	apk add --no-cache 		apr 		apr-util 		apr-util-ldap 		ca-certificates 		perl 	;
# Mon, 13 Mar 2023 16:45:43 GMT
ENV HTTPD_VERSION=2.4.56
# Mon, 13 Mar 2023 16:45:43 GMT
ENV HTTPD_SHA256=d8d45f1398ba84edd05bb33ca7593ac2989b17cb9c7a0cafe5442d41afdb2d7c
# Mon, 13 Mar 2023 16:45:43 GMT
ENV HTTPD_PATCHES=
# Mon, 13 Mar 2023 16:46:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		apr-dev 		apr-util-dev 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://downloads.apache.org/ 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		DE29FB3971E71543FD2DC049508EAEC5302DA568 		13155B0E9E634F42BF6C163FDDBA64BA2C312D2F 		8B39757B1D8A994DF2433ED58B3A601F08C975E5 		31EE1A81B8D066548156D37B7D6DBFD1F08E012A 		A10208FEC3152DD7C0C9B59B361522D782AB7BD1 		3DE024AFDA7A4B15CB6C14410F81AA8AB0D5F771 		EB138C6AF0FC691001B16D93344A844D751D7F27 		CBA5A7C21EC143314C41393E5B968010E04F9A89 		3C016F2B764621BB549C66B516A96495E2226795 		937FB3994A242BA9BF49E93021454AF0CC8B0F7E 		EAD1359A4C0F2D37472AAF28F55DF0293A4E7AC9 		4C1EADADB4EF5007579C919C6635B6C0DE885DD3 		01E475360FCCF1D0F24B9D145D414AE1E005C9CB 		92CCEF0AA7DD46AC3A0F498BCA6939748103A37E 		D395C7573A68B9796D38C258153FA0CD75A67692 		FA39B617B61493FD283503E7EED1EA392261D073 		984FB3350C1D5C7A3282255BB31B213D208F5064 		FE7A49DAA875E890B4167F76CCB2EB46E76CF6D0 		39F6691A0ECF0C50E8BB849CF78875F642721F00 		29A2BA848177B73878277FA475CAA2A3F39B3750 		120A8667241AEDD4A78B46104C042818311A3DE5 		453510BDA6C5855624E009236D0BC73A40581837 		0DE5C55C6BF3B2352DABB89E13249B4FEC88A0BF 		7CDBED100806552182F98844E8E7E00B4DAA1988 		A8BA9617EF3BCCAC3B29B869EDB105896F9522D8 		3E6AC004854F3A7F03566B592FF06894E55B0D0E 		5B5181C2C0AB13E59DA3F7A3EC582EB639FF092C 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		65B2D44FE74BD5E3DE3AC3F082781DE46D5954FA 		8935926745E1CE7E3ED748F6EC99EE267EB5F61A 		E3480043595621FE56105F112AB12A7ADC55C003 		93525CFCF6FDFFB3FD9700DD5A4B10AE43B56A27 		C55AB7B9139EB2263CD1AABC19B033D1760C227B 		26F51EF9A82F4ACB43F1903ED377C9E7D1944C66 	; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*User)\s+daemon\s*$!\1 www-data!g' 		-e 's!^(\s*Group)\s+daemon\s*$!\1 www-data!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 	grep -E '^\s*User www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 	grep -E '^\s*Group www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 		deps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-so-deps $deps; 	apk del --no-network .build-deps; 		httpd -v
# Mon, 13 Mar 2023 16:46:54 GMT
STOPSIGNAL SIGWINCH
# Mon, 13 Mar 2023 16:46:54 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Mon, 13 Mar 2023 16:46:54 GMT
EXPOSE 80
# Mon, 13 Mar 2023 16:46:54 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:6a6e4ab63e54442e16400f69d37f662d60cbd67565631eff6bf59b4176e482c3`  
		Last Modified: Fri, 10 Feb 2023 20:50:22 GMT  
		Size: 3.1 MB (3110885 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2695e20dbd2f3b0b796921bc9dc1531c3adadad205b06106158854119d58e39`  
		Last Modified: Mon, 13 Mar 2023 16:47:22 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5f74ea456ad7466116805f19d78cdb70bb818342bdf7fc7dc9b6ca49ce85bd2`  
		Last Modified: Mon, 13 Mar 2023 16:47:22 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48b40135fffd1a5f11a54f42ab0621406e8c4c0fed3c83ef7ce7201d86813df1`  
		Last Modified: Mon, 13 Mar 2023 16:47:24 GMT  
		Size: 9.2 MB (9153488 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a3cd5e814decb65d24f6b662b98c7c04e95638164cc7ff2cfffbab569331de3`  
		Last Modified: Mon, 13 Mar 2023 16:47:23 GMT  
		Size: 4.3 MB (4308772 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3da689e74571ed2516b83e5c8f2e234b7b2f4b509b7eb1f2d11baff42dfa2fff`  
		Last Modified: Mon, 13 Mar 2023 16:47:22 GMT  
		Size: 294.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; arm variant v7

```console
$ docker pull httpd@sha256:eb186fe9b0cfd531e3fe7ec3be398d7f48370b16546b1382d32ef91209f466a6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **15.9 MB (15856258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a177cd4ca20715a6c89447b3a8abf042ac7d07953daa1cece1bad6ade6199fc3`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Fri, 10 Feb 2023 21:51:31 GMT
ADD file:143b601fcc6b5d7d95d3e5ccad3fec7081191a47e28d4f9294a7fb2499cab1af in / 
# Fri, 10 Feb 2023 21:51:31 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 05:21:37 GMT
RUN set -x 	&& adduser -u 82 -D -S -G www-data www-data
# Wed, 01 Mar 2023 05:21:37 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Wed, 01 Mar 2023 05:21:37 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 05:21:37 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Wed, 01 Mar 2023 05:21:37 GMT
WORKDIR /usr/local/apache2
# Wed, 01 Mar 2023 05:21:40 GMT
RUN set -eux; 	apk add --no-cache 		apr 		apr-util 		apr-util-ldap 		ca-certificates 		perl 	;
# Tue, 07 Mar 2023 20:04:02 GMT
ENV HTTPD_VERSION=2.4.56
# Tue, 07 Mar 2023 20:04:02 GMT
ENV HTTPD_SHA256=d8d45f1398ba84edd05bb33ca7593ac2989b17cb9c7a0cafe5442d41afdb2d7c
# Tue, 07 Mar 2023 20:04:02 GMT
ENV HTTPD_PATCHES=
# Tue, 07 Mar 2023 20:05:16 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		apr-dev 		apr-util-dev 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://downloads.apache.org/ 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		DE29FB3971E71543FD2DC049508EAEC5302DA568 		13155B0E9E634F42BF6C163FDDBA64BA2C312D2F 		8B39757B1D8A994DF2433ED58B3A601F08C975E5 		31EE1A81B8D066548156D37B7D6DBFD1F08E012A 		A10208FEC3152DD7C0C9B59B361522D782AB7BD1 		3DE024AFDA7A4B15CB6C14410F81AA8AB0D5F771 		EB138C6AF0FC691001B16D93344A844D751D7F27 		CBA5A7C21EC143314C41393E5B968010E04F9A89 		3C016F2B764621BB549C66B516A96495E2226795 		937FB3994A242BA9BF49E93021454AF0CC8B0F7E 		EAD1359A4C0F2D37472AAF28F55DF0293A4E7AC9 		4C1EADADB4EF5007579C919C6635B6C0DE885DD3 		01E475360FCCF1D0F24B9D145D414AE1E005C9CB 		92CCEF0AA7DD46AC3A0F498BCA6939748103A37E 		D395C7573A68B9796D38C258153FA0CD75A67692 		FA39B617B61493FD283503E7EED1EA392261D073 		984FB3350C1D5C7A3282255BB31B213D208F5064 		FE7A49DAA875E890B4167F76CCB2EB46E76CF6D0 		39F6691A0ECF0C50E8BB849CF78875F642721F00 		29A2BA848177B73878277FA475CAA2A3F39B3750 		120A8667241AEDD4A78B46104C042818311A3DE5 		453510BDA6C5855624E009236D0BC73A40581837 		0DE5C55C6BF3B2352DABB89E13249B4FEC88A0BF 		7CDBED100806552182F98844E8E7E00B4DAA1988 		A8BA9617EF3BCCAC3B29B869EDB105896F9522D8 		3E6AC004854F3A7F03566B592FF06894E55B0D0E 		5B5181C2C0AB13E59DA3F7A3EC582EB639FF092C 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		65B2D44FE74BD5E3DE3AC3F082781DE46D5954FA 		8935926745E1CE7E3ED748F6EC99EE267EB5F61A 		E3480043595621FE56105F112AB12A7ADC55C003 		93525CFCF6FDFFB3FD9700DD5A4B10AE43B56A27 		C55AB7B9139EB2263CD1AABC19B033D1760C227B 		26F51EF9A82F4ACB43F1903ED377C9E7D1944C66 	; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*User)\s+daemon\s*$!\1 www-data!g' 		-e 's!^(\s*Group)\s+daemon\s*$!\1 www-data!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 	grep -E '^\s*User www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 	grep -E '^\s*Group www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 		deps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-so-deps $deps; 	apk del --no-network .build-deps; 		httpd -v
# Tue, 07 Mar 2023 20:05:17 GMT
STOPSIGNAL SIGWINCH
# Tue, 07 Mar 2023 20:05:17 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Tue, 07 Mar 2023 20:05:17 GMT
EXPOSE 80
# Tue, 07 Mar 2023 20:05:17 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:6fb81ff47bd6d7db0ed86c9b951ad6417ec73ab60af6d22daa604076a902629c`  
		Last Modified: Fri, 10 Feb 2023 21:52:33 GMT  
		Size: 2.9 MB (2868494 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99d41b7c9ef868cc29c3733558a70cfa3ba5e2b6f198800f8e93d49a41d1c978`  
		Last Modified: Wed, 01 Mar 2023 05:24:08 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dfd81498dc0b9bd9384e34208237208d767b94a6f8e8551f797fc740e5b42c37`  
		Last Modified: Wed, 01 Mar 2023 05:24:08 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9631cbd7ecd7d4ceb92167226ba8c36c643c00e7fd2306465cf0fe5af315118`  
		Last Modified: Wed, 01 Mar 2023 05:24:10 GMT  
		Size: 9.0 MB (8952693 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eaad147ebefe2f1673018f3ac67322bdf8a86010ce3ff0aec2174d2d382d0b69`  
		Last Modified: Tue, 07 Mar 2023 20:06:39 GMT  
		Size: 4.0 MB (4033331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667818e4c8127050549c3d6082f765c723ac0c6f2cc53e6dc920da1bcb3e1610`  
		Last Modified: Tue, 07 Mar 2023 20:06:38 GMT  
		Size: 300.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; arm64 variant v8

```console
$ docker pull httpd@sha256:b6c0c3625edc1eba6d9b84caf33b87d1d18fe0147fbe1496acec74c25902a667
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.4 MB (17430008 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b34bdf4ecb0ec9332be9661b048d7892221efa6247da1abacbb5662dd5e20d1b`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:08 GMT
ADD file:9bd9ea42a9f3bdc769e80c6b8a4b117d65f73ae68e155a6172a1184e7ac8bcc1 in / 
# Fri, 10 Feb 2023 21:24:08 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:52:28 GMT
RUN set -x 	&& adduser -u 82 -D -S -G www-data www-data
# Fri, 10 Feb 2023 22:52:28 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Fri, 10 Feb 2023 22:52:28 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Feb 2023 22:52:29 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Fri, 10 Feb 2023 22:52:29 GMT
WORKDIR /usr/local/apache2
# Fri, 10 Feb 2023 22:52:30 GMT
RUN set -eux; 	apk add --no-cache 		apr 		apr-util 		apr-util-ldap 		ca-certificates 		perl 	;
# Tue, 07 Mar 2023 19:48:20 GMT
ENV HTTPD_VERSION=2.4.56
# Tue, 07 Mar 2023 19:48:20 GMT
ENV HTTPD_SHA256=d8d45f1398ba84edd05bb33ca7593ac2989b17cb9c7a0cafe5442d41afdb2d7c
# Tue, 07 Mar 2023 19:48:20 GMT
ENV HTTPD_PATCHES=
# Tue, 07 Mar 2023 19:49:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		apr-dev 		apr-util-dev 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://downloads.apache.org/ 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		DE29FB3971E71543FD2DC049508EAEC5302DA568 		13155B0E9E634F42BF6C163FDDBA64BA2C312D2F 		8B39757B1D8A994DF2433ED58B3A601F08C975E5 		31EE1A81B8D066548156D37B7D6DBFD1F08E012A 		A10208FEC3152DD7C0C9B59B361522D782AB7BD1 		3DE024AFDA7A4B15CB6C14410F81AA8AB0D5F771 		EB138C6AF0FC691001B16D93344A844D751D7F27 		CBA5A7C21EC143314C41393E5B968010E04F9A89 		3C016F2B764621BB549C66B516A96495E2226795 		937FB3994A242BA9BF49E93021454AF0CC8B0F7E 		EAD1359A4C0F2D37472AAF28F55DF0293A4E7AC9 		4C1EADADB4EF5007579C919C6635B6C0DE885DD3 		01E475360FCCF1D0F24B9D145D414AE1E005C9CB 		92CCEF0AA7DD46AC3A0F498BCA6939748103A37E 		D395C7573A68B9796D38C258153FA0CD75A67692 		FA39B617B61493FD283503E7EED1EA392261D073 		984FB3350C1D5C7A3282255BB31B213D208F5064 		FE7A49DAA875E890B4167F76CCB2EB46E76CF6D0 		39F6691A0ECF0C50E8BB849CF78875F642721F00 		29A2BA848177B73878277FA475CAA2A3F39B3750 		120A8667241AEDD4A78B46104C042818311A3DE5 		453510BDA6C5855624E009236D0BC73A40581837 		0DE5C55C6BF3B2352DABB89E13249B4FEC88A0BF 		7CDBED100806552182F98844E8E7E00B4DAA1988 		A8BA9617EF3BCCAC3B29B869EDB105896F9522D8 		3E6AC004854F3A7F03566B592FF06894E55B0D0E 		5B5181C2C0AB13E59DA3F7A3EC582EB639FF092C 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		65B2D44FE74BD5E3DE3AC3F082781DE46D5954FA 		8935926745E1CE7E3ED748F6EC99EE267EB5F61A 		E3480043595621FE56105F112AB12A7ADC55C003 		93525CFCF6FDFFB3FD9700DD5A4B10AE43B56A27 		C55AB7B9139EB2263CD1AABC19B033D1760C227B 		26F51EF9A82F4ACB43F1903ED377C9E7D1944C66 	; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*User)\s+daemon\s*$!\1 www-data!g' 		-e 's!^(\s*Group)\s+daemon\s*$!\1 www-data!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 	grep -E '^\s*User www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 	grep -E '^\s*Group www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 		deps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-so-deps $deps; 	apk del --no-network .build-deps; 		httpd -v
# Tue, 07 Mar 2023 19:49:22 GMT
STOPSIGNAL SIGWINCH
# Tue, 07 Mar 2023 19:49:22 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Tue, 07 Mar 2023 19:49:22 GMT
EXPOSE 80
# Tue, 07 Mar 2023 19:49:22 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:af6eaf76a39c2d3e7e0b8a0420486e3df33c4027d696c076a99a3d0ac09026af`  
		Last Modified: Fri, 10 Feb 2023 21:24:39 GMT  
		Size: 3.3 MB (3261959 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7cf8be70a441746af327deffe2ffedac4080bac66f1d03b0d596ece7e9f09e4`  
		Last Modified: Fri, 10 Feb 2023 22:53:58 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c56b9eb9b9dfd91231816f800655f44bb57ae09e85ee7e9eadf5a29d3e426ea2`  
		Last Modified: Fri, 10 Feb 2023 22:53:58 GMT  
		Size: 176.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:190df969b5fac5571cf929b5ddb2916761d454eee02a1fe1a6703e39fd49dd57`  
		Last Modified: Fri, 10 Feb 2023 22:54:00 GMT  
		Size: 9.9 MB (9913721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0b9469bcc6f3b55b0e990bd2e72c8b7930db270fb81a2c09a4b458eebd48a91`  
		Last Modified: Tue, 07 Mar 2023 19:50:14 GMT  
		Size: 4.3 MB (4252594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a99608181b3cb0fd00dc12de1d07c9b20aac28eeaac053d3aaaf592f4dcae8b8`  
		Last Modified: Tue, 07 Mar 2023 19:50:13 GMT  
		Size: 297.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; 386

```console
$ docker pull httpd@sha256:e4498843f8684e957e3068546ed930b30d43180e2e8c2579d39d637bd2fe79de
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.9 MB (16906859 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c17cd075848397f28c6ffe5f48a0520dbfe7556c6eb65fe73d08657fc0ccf28`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:23 GMT
ADD file:125f3514520a5cd29df2830a409aa026a2bc06a77a7a5d150133436404b33d41 in / 
# Fri, 10 Feb 2023 21:24:24 GMT
CMD ["/bin/sh"]
# Wed, 01 Mar 2023 09:26:02 GMT
RUN set -x 	&& adduser -u 82 -D -S -G www-data www-data
# Wed, 01 Mar 2023 09:26:02 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Wed, 01 Mar 2023 09:26:02 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Mar 2023 09:26:02 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Wed, 01 Mar 2023 09:26:02 GMT
WORKDIR /usr/local/apache2
# Wed, 01 Mar 2023 09:26:06 GMT
RUN set -eux; 	apk add --no-cache 		apr 		apr-util 		apr-util-ldap 		ca-certificates 		perl 	;
# Tue, 07 Mar 2023 19:47:54 GMT
ENV HTTPD_VERSION=2.4.56
# Tue, 07 Mar 2023 19:47:55 GMT
ENV HTTPD_SHA256=d8d45f1398ba84edd05bb33ca7593ac2989b17cb9c7a0cafe5442d41afdb2d7c
# Tue, 07 Mar 2023 19:47:55 GMT
ENV HTTPD_PATCHES=
# Tue, 07 Mar 2023 19:49:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		apr-dev 		apr-util-dev 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://downloads.apache.org/ 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		DE29FB3971E71543FD2DC049508EAEC5302DA568 		13155B0E9E634F42BF6C163FDDBA64BA2C312D2F 		8B39757B1D8A994DF2433ED58B3A601F08C975E5 		31EE1A81B8D066548156D37B7D6DBFD1F08E012A 		A10208FEC3152DD7C0C9B59B361522D782AB7BD1 		3DE024AFDA7A4B15CB6C14410F81AA8AB0D5F771 		EB138C6AF0FC691001B16D93344A844D751D7F27 		CBA5A7C21EC143314C41393E5B968010E04F9A89 		3C016F2B764621BB549C66B516A96495E2226795 		937FB3994A242BA9BF49E93021454AF0CC8B0F7E 		EAD1359A4C0F2D37472AAF28F55DF0293A4E7AC9 		4C1EADADB4EF5007579C919C6635B6C0DE885DD3 		01E475360FCCF1D0F24B9D145D414AE1E005C9CB 		92CCEF0AA7DD46AC3A0F498BCA6939748103A37E 		D395C7573A68B9796D38C258153FA0CD75A67692 		FA39B617B61493FD283503E7EED1EA392261D073 		984FB3350C1D5C7A3282255BB31B213D208F5064 		FE7A49DAA875E890B4167F76CCB2EB46E76CF6D0 		39F6691A0ECF0C50E8BB849CF78875F642721F00 		29A2BA848177B73878277FA475CAA2A3F39B3750 		120A8667241AEDD4A78B46104C042818311A3DE5 		453510BDA6C5855624E009236D0BC73A40581837 		0DE5C55C6BF3B2352DABB89E13249B4FEC88A0BF 		7CDBED100806552182F98844E8E7E00B4DAA1988 		A8BA9617EF3BCCAC3B29B869EDB105896F9522D8 		3E6AC004854F3A7F03566B592FF06894E55B0D0E 		5B5181C2C0AB13E59DA3F7A3EC582EB639FF092C 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		65B2D44FE74BD5E3DE3AC3F082781DE46D5954FA 		8935926745E1CE7E3ED748F6EC99EE267EB5F61A 		E3480043595621FE56105F112AB12A7ADC55C003 		93525CFCF6FDFFB3FD9700DD5A4B10AE43B56A27 		C55AB7B9139EB2263CD1AABC19B033D1760C227B 		26F51EF9A82F4ACB43F1903ED377C9E7D1944C66 	; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*User)\s+daemon\s*$!\1 www-data!g' 		-e 's!^(\s*Group)\s+daemon\s*$!\1 www-data!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 	grep -E '^\s*User www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 	grep -E '^\s*Group www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 		deps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-so-deps $deps; 	apk del --no-network .build-deps; 		httpd -v
# Tue, 07 Mar 2023 19:49:26 GMT
STOPSIGNAL SIGWINCH
# Tue, 07 Mar 2023 19:49:26 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Tue, 07 Mar 2023 19:49:26 GMT
EXPOSE 80
# Tue, 07 Mar 2023 19:49:26 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:b3e346c15c2377ec0e75cc9efa98baecd58b0e9bb92f0ec07eeda0bcc7e67fc7`  
		Last Modified: Fri, 10 Feb 2023 21:25:13 GMT  
		Size: 3.4 MB (3412353 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9111bb4a8aaae1f21c99ab554871e7e525038e743e6be81bf35c27a77c59b6f`  
		Last Modified: Wed, 01 Mar 2023 09:29:01 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:11031a9049912d69504390064a19080196632dca6a1e6542c2d2e09d938b5aff`  
		Last Modified: Wed, 01 Mar 2023 09:29:01 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:310fa094709f8303c6f5a740611d8482ff2cf0d8b5a8c52a3c988d339c2e5dd2`  
		Last Modified: Wed, 01 Mar 2023 09:29:04 GMT  
		Size: 9.3 MB (9312328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80c9d2f03d936530fd166a523873993f4fb413ec0cc98f3ac439ea05dacbd571`  
		Last Modified: Tue, 07 Mar 2023 19:50:42 GMT  
		Size: 4.2 MB (4180441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:417e5f7d2f0d4e9ceb39ba42397187514058d7a255b7f117409035498c025cbf`  
		Last Modified: Tue, 07 Mar 2023 19:50:41 GMT  
		Size: 299.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; ppc64le

```console
$ docker pull httpd@sha256:8c92917e78775a8f1f27fd6c03da4d2262697a35e7c3d6f2e596178f5a9c2ae0
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 MB (17878283 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0d3a63929f4e2aeb15cced70ba792628ee641647dd0866dfccab3555ede64035`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Fri, 10 Feb 2023 21:20:36 GMT
ADD file:ec037a0d4b462d12963ac20d9ec49bb73b4bcaf84d4bc7b364ebf93667e585b0 in / 
# Fri, 10 Feb 2023 21:20:36 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:27:59 GMT
RUN set -x 	&& adduser -u 82 -D -S -G www-data www-data
# Sat, 11 Feb 2023 09:28:00 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Sat, 11 Feb 2023 09:28:00 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 11 Feb 2023 09:28:01 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Sat, 11 Feb 2023 09:28:02 GMT
WORKDIR /usr/local/apache2
# Sat, 11 Feb 2023 09:28:07 GMT
RUN set -eux; 	apk add --no-cache 		apr 		apr-util 		apr-util-ldap 		ca-certificates 		perl 	;
# Tue, 07 Mar 2023 20:25:54 GMT
ENV HTTPD_VERSION=2.4.56
# Tue, 07 Mar 2023 20:25:54 GMT
ENV HTTPD_SHA256=d8d45f1398ba84edd05bb33ca7593ac2989b17cb9c7a0cafe5442d41afdb2d7c
# Tue, 07 Mar 2023 20:25:55 GMT
ENV HTTPD_PATCHES=
# Tue, 07 Mar 2023 20:27:59 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		apr-dev 		apr-util-dev 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://downloads.apache.org/ 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		DE29FB3971E71543FD2DC049508EAEC5302DA568 		13155B0E9E634F42BF6C163FDDBA64BA2C312D2F 		8B39757B1D8A994DF2433ED58B3A601F08C975E5 		31EE1A81B8D066548156D37B7D6DBFD1F08E012A 		A10208FEC3152DD7C0C9B59B361522D782AB7BD1 		3DE024AFDA7A4B15CB6C14410F81AA8AB0D5F771 		EB138C6AF0FC691001B16D93344A844D751D7F27 		CBA5A7C21EC143314C41393E5B968010E04F9A89 		3C016F2B764621BB549C66B516A96495E2226795 		937FB3994A242BA9BF49E93021454AF0CC8B0F7E 		EAD1359A4C0F2D37472AAF28F55DF0293A4E7AC9 		4C1EADADB4EF5007579C919C6635B6C0DE885DD3 		01E475360FCCF1D0F24B9D145D414AE1E005C9CB 		92CCEF0AA7DD46AC3A0F498BCA6939748103A37E 		D395C7573A68B9796D38C258153FA0CD75A67692 		FA39B617B61493FD283503E7EED1EA392261D073 		984FB3350C1D5C7A3282255BB31B213D208F5064 		FE7A49DAA875E890B4167F76CCB2EB46E76CF6D0 		39F6691A0ECF0C50E8BB849CF78875F642721F00 		29A2BA848177B73878277FA475CAA2A3F39B3750 		120A8667241AEDD4A78B46104C042818311A3DE5 		453510BDA6C5855624E009236D0BC73A40581837 		0DE5C55C6BF3B2352DABB89E13249B4FEC88A0BF 		7CDBED100806552182F98844E8E7E00B4DAA1988 		A8BA9617EF3BCCAC3B29B869EDB105896F9522D8 		3E6AC004854F3A7F03566B592FF06894E55B0D0E 		5B5181C2C0AB13E59DA3F7A3EC582EB639FF092C 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		65B2D44FE74BD5E3DE3AC3F082781DE46D5954FA 		8935926745E1CE7E3ED748F6EC99EE267EB5F61A 		E3480043595621FE56105F112AB12A7ADC55C003 		93525CFCF6FDFFB3FD9700DD5A4B10AE43B56A27 		C55AB7B9139EB2263CD1AABC19B033D1760C227B 		26F51EF9A82F4ACB43F1903ED377C9E7D1944C66 	; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*User)\s+daemon\s*$!\1 www-data!g' 		-e 's!^(\s*Group)\s+daemon\s*$!\1 www-data!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 	grep -E '^\s*User www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 	grep -E '^\s*Group www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 		deps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-so-deps $deps; 	apk del --no-network .build-deps; 		httpd -v
# Tue, 07 Mar 2023 20:28:00 GMT
STOPSIGNAL SIGWINCH
# Tue, 07 Mar 2023 20:28:00 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Tue, 07 Mar 2023 20:28:01 GMT
EXPOSE 80
# Tue, 07 Mar 2023 20:28:01 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:aa3c56f9c6f127b6c8f628c95db165741ca400d19bdaef2752d80f093e47451e`  
		Last Modified: Fri, 10 Feb 2023 21:21:37 GMT  
		Size: 3.4 MB (3390750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c3b12513a207ec25eb3c7061abdfdf41e690b079dae65ff1e1735a8e12d3904`  
		Last Modified: Sat, 11 Feb 2023 09:31:05 GMT  
		Size: 1.3 KB (1263 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0214a524218e6de8801c3e4a60f77554a7fc6b8675c9be453051800011ca611a`  
		Last Modified: Sat, 11 Feb 2023 09:31:05 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1850c13cb6bb9bab0d89153d07b06a6a41f6fa71c7ef814476e1b58206cac1a0`  
		Last Modified: Sat, 11 Feb 2023 09:31:09 GMT  
		Size: 10.0 MB (10005502 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68448e2a81d3a895b5e1598e293c26d802f5bbedd0046483e0a424360afb3301`  
		Last Modified: Tue, 07 Mar 2023 20:29:27 GMT  
		Size: 4.5 MB (4480292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1e293d2be00f9fc6e57ffbc5c3df9d57ee3ed3f51b65ce9ade16cc7c5336575`  
		Last Modified: Tue, 07 Mar 2023 20:29:25 GMT  
		Size: 299.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; s390x

```console
$ docker pull httpd@sha256:3ae8dd7de4568e384121fad202ae0ac500db28ca8a9d08defbee40b88886aa14
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17723816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d405e70d283efb5757ca8b2ff5937294ebb1da47368949e823ddf4a35b4b3caa`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Fri, 10 Feb 2023 21:41:25 GMT
ADD file:03b2fb4d732a294329449ff55c5d84f7d2735e6510985718979469994f3a607b in / 
# Fri, 10 Feb 2023 21:41:26 GMT
CMD ["/bin/sh"]
# Fri, 10 Feb 2023 22:39:25 GMT
RUN set -x 	&& adduser -u 82 -D -S -G www-data www-data
# Fri, 10 Feb 2023 22:39:25 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Fri, 10 Feb 2023 22:39:25 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Fri, 10 Feb 2023 22:39:26 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Fri, 10 Feb 2023 22:39:26 GMT
WORKDIR /usr/local/apache2
# Fri, 10 Feb 2023 22:39:29 GMT
RUN set -eux; 	apk add --no-cache 		apr 		apr-util 		apr-util-ldap 		ca-certificates 		perl 	;
# Tue, 07 Mar 2023 19:48:04 GMT
ENV HTTPD_VERSION=2.4.56
# Tue, 07 Mar 2023 19:48:04 GMT
ENV HTTPD_SHA256=d8d45f1398ba84edd05bb33ca7593ac2989b17cb9c7a0cafe5442d41afdb2d7c
# Tue, 07 Mar 2023 19:48:04 GMT
ENV HTTPD_PATCHES=
# Tue, 07 Mar 2023 19:49:01 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		apr-dev 		apr-util-dev 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://downloads.apache.org/ 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		DE29FB3971E71543FD2DC049508EAEC5302DA568 		13155B0E9E634F42BF6C163FDDBA64BA2C312D2F 		8B39757B1D8A994DF2433ED58B3A601F08C975E5 		31EE1A81B8D066548156D37B7D6DBFD1F08E012A 		A10208FEC3152DD7C0C9B59B361522D782AB7BD1 		3DE024AFDA7A4B15CB6C14410F81AA8AB0D5F771 		EB138C6AF0FC691001B16D93344A844D751D7F27 		CBA5A7C21EC143314C41393E5B968010E04F9A89 		3C016F2B764621BB549C66B516A96495E2226795 		937FB3994A242BA9BF49E93021454AF0CC8B0F7E 		EAD1359A4C0F2D37472AAF28F55DF0293A4E7AC9 		4C1EADADB4EF5007579C919C6635B6C0DE885DD3 		01E475360FCCF1D0F24B9D145D414AE1E005C9CB 		92CCEF0AA7DD46AC3A0F498BCA6939748103A37E 		D395C7573A68B9796D38C258153FA0CD75A67692 		FA39B617B61493FD283503E7EED1EA392261D073 		984FB3350C1D5C7A3282255BB31B213D208F5064 		FE7A49DAA875E890B4167F76CCB2EB46E76CF6D0 		39F6691A0ECF0C50E8BB849CF78875F642721F00 		29A2BA848177B73878277FA475CAA2A3F39B3750 		120A8667241AEDD4A78B46104C042818311A3DE5 		453510BDA6C5855624E009236D0BC73A40581837 		0DE5C55C6BF3B2352DABB89E13249B4FEC88A0BF 		7CDBED100806552182F98844E8E7E00B4DAA1988 		A8BA9617EF3BCCAC3B29B869EDB105896F9522D8 		3E6AC004854F3A7F03566B592FF06894E55B0D0E 		5B5181C2C0AB13E59DA3F7A3EC582EB639FF092C 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		65B2D44FE74BD5E3DE3AC3F082781DE46D5954FA 		8935926745E1CE7E3ED748F6EC99EE267EB5F61A 		E3480043595621FE56105F112AB12A7ADC55C003 		93525CFCF6FDFFB3FD9700DD5A4B10AE43B56A27 		C55AB7B9139EB2263CD1AABC19B033D1760C227B 		26F51EF9A82F4ACB43F1903ED377C9E7D1944C66 	; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*User)\s+daemon\s*$!\1 www-data!g' 		-e 's!^(\s*Group)\s+daemon\s*$!\1 www-data!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 	grep -E '^\s*User www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 	grep -E '^\s*Group www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 		deps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-so-deps $deps; 	apk del --no-network .build-deps; 		httpd -v
# Tue, 07 Mar 2023 19:49:01 GMT
STOPSIGNAL SIGWINCH
# Tue, 07 Mar 2023 19:49:01 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Tue, 07 Mar 2023 19:49:01 GMT
EXPOSE 80
# Tue, 07 Mar 2023 19:49:01 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:24c4f8de3549a39c64b0edc2cfa68769b373f35138d0f13725100160bb32d4e2`  
		Last Modified: Fri, 10 Feb 2023 21:42:16 GMT  
		Size: 3.2 MB (3175116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4c95ea3b95832401e20b2e8f4ff07fcff515643c0bba79b2023fd80648debfe`  
		Last Modified: Fri, 10 Feb 2023 22:41:22 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ed1180606b37a433f62b226ca61a18d1e27d099e7cda56d6f00a177d27e0af6`  
		Last Modified: Fri, 10 Feb 2023 22:41:22 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84d666abab0f57ebea520d07076c12e50e08884a5559cb8a845ab5ab226cd2b5`  
		Last Modified: Fri, 10 Feb 2023 22:41:24 GMT  
		Size: 10.3 MB (10330455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33aaaea27136718b8827ee2da6bb66dcd036e67fe199294837dd65eafa9e947d`  
		Last Modified: Tue, 07 Mar 2023 19:50:00 GMT  
		Size: 4.2 MB (4216505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c1c67b14d803480e179e884646a1593885ac464a7c1867268499972d2897c39`  
		Last Modified: Tue, 07 Mar 2023 19:49:59 GMT  
		Size: 300.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
