## `httpd:2-alpine`

```console
$ docker pull httpd@sha256:eead66760a36f645895bd683d415ce50c0b944fd9270ad4fcfbc25bf2cb88933
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
$ docker pull httpd@sha256:4a0516793d26a35e4a3bc6d1666ea204e5122d62d96b0f502595b82e5454bfff
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18274650 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:798f120eb327c87f30a3a94d6100a57c263097d2c2b64a27fe3f0a47adb75809`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:40:19 GMT
RUN set -x 	&& adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 04:40:19 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Tue, 30 Nov 2021 04:40:19 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 04:40:20 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Tue, 30 Nov 2021 04:40:20 GMT
WORKDIR /usr/local/apache2
# Tue, 30 Nov 2021 04:40:23 GMT
RUN set -eux; 	apk add --no-cache 		apr 		apr-util 		apr-util-ldap 		perl 	;
# Mon, 14 Mar 2022 19:17:01 GMT
ENV HTTPD_VERSION=2.4.53
# Mon, 14 Mar 2022 19:17:01 GMT
ENV HTTPD_SHA256=d0bbd1121a57b5f2a6ff92d7b96f8050c5a45d3f14db118f64979d525858db63
# Mon, 14 Mar 2022 19:17:01 GMT
ENV HTTPD_PATCHES=
# Mon, 14 Mar 2022 19:19:43 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		apr-dev 		apr-util-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://downloads.apache.org/ 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		DE29FB3971E71543FD2DC049508EAEC5302DA568 		13155B0E9E634F42BF6C163FDDBA64BA2C312D2F 		8B39757B1D8A994DF2433ED58B3A601F08C975E5 		31EE1A81B8D066548156D37B7D6DBFD1F08E012A 		A10208FEC3152DD7C0C9B59B361522D782AB7BD1 		3DE024AFDA7A4B15CB6C14410F81AA8AB0D5F771 		EB138C6AF0FC691001B16D93344A844D751D7F27 		CBA5A7C21EC143314C41393E5B968010E04F9A89 		3C016F2B764621BB549C66B516A96495E2226795 		937FB3994A242BA9BF49E93021454AF0CC8B0F7E 		EAD1359A4C0F2D37472AAF28F55DF0293A4E7AC9 		4C1EADADB4EF5007579C919C6635B6C0DE885DD3 		01E475360FCCF1D0F24B9D145D414AE1E005C9CB 		92CCEF0AA7DD46AC3A0F498BCA6939748103A37E 		D395C7573A68B9796D38C258153FA0CD75A67692 		FA39B617B61493FD283503E7EED1EA392261D073 		984FB3350C1D5C7A3282255BB31B213D208F5064 		FE7A49DAA875E890B4167F76CCB2EB46E76CF6D0 		39F6691A0ECF0C50E8BB849CF78875F642721F00 		29A2BA848177B73878277FA475CAA2A3F39B3750 		120A8667241AEDD4A78B46104C042818311A3DE5 		453510BDA6C5855624E009236D0BC73A40581837 		0DE5C55C6BF3B2352DABB89E13249B4FEC88A0BF 		7CDBED100806552182F98844E8E7E00B4DAA1988 		A8BA9617EF3BCCAC3B29B869EDB105896F9522D8 		3E6AC004854F3A7F03566B592FF06894E55B0D0E 		5B5181C2C0AB13E59DA3F7A3EC582EB639FF092C 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		65B2D44FE74BD5E3DE3AC3F082781DE46D5954FA 		8935926745E1CE7E3ED748F6EC99EE267EB5F61A 		E3480043595621FE56105F112AB12A7ADC55C003 		93525CFCF6FDFFB3FD9700DD5A4B10AE43B56A27 		C55AB7B9139EB2263CD1AABC19B033D1760C227B 		26F51EF9A82F4ACB43F1903ED377C9E7D1944C66 	; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*User)\s+daemon\s*$!\1 www-data!g' 		-e 's!^(\s*Group)\s+daemon\s*$!\1 www-data!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 	grep -E '^\s*User www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 	grep -E '^\s*Group www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 		deps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-so-deps $deps; 	apk del --no-network .build-deps; 		httpd -v
# Mon, 14 Mar 2022 19:19:43 GMT
STOPSIGNAL SIGWINCH
# Mon, 14 Mar 2022 19:19:43 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Mon, 14 Mar 2022 19:19:43 GMT
EXPOSE 80
# Mon, 14 Mar 2022 19:19:43 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085d9bf42ab2b96f1ec8996ee4ef722d286dbbfd0f6f17f5260ff7d806696483`  
		Last Modified: Tue, 30 Nov 2021 04:42:46 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:907dfa98a03e7a3aeba43eb32d4368e8dd241c68b19bc3e987b98b0daa824d37`  
		Last Modified: Tue, 30 Nov 2021 04:42:46 GMT  
		Size: 179.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:242407d61b32dc78c58733d64c99c2f3441a140f7f5a8d38c93cfc16a5cb73e8`  
		Last Modified: Tue, 30 Nov 2021 04:42:48 GMT  
		Size: 9.5 MB (9529609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:16b7c5d0738c7d40cc8d80d76b89432290a3e6d9ccdd86dc021bf6b5b77077a9`  
		Last Modified: Mon, 14 Mar 2022 19:20:38 GMT  
		Size: 5.9 MB (5924894 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f570a2d80397d6ec45ec7d3a7b851d9ee0aba05d6cb5cf5187b1438d3154b6d3`  
		Last Modified: Mon, 14 Mar 2022 19:20:37 GMT  
		Size: 299.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; arm variant v6

```console
$ docker pull httpd@sha256:51a6d85853f99f4eed5fe70b7209ac3b0e95eb0d586170a607d084a63b1b5090
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.0 MB (16979562 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:751158748c1fd09a64b53601afa74c00af7778f1949cac8427d824f8c2f8a05e`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Wed, 24 Nov 2021 21:08:16 GMT
ADD file:61137e0aa49ba06f57ac69466fe2fb116f580b5e6159d56f846b1d72c4a3c814 in / 
# Wed, 24 Nov 2021 21:08:16 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 03:14:20 GMT
RUN set -x 	&& adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 03:14:21 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Tue, 30 Nov 2021 03:14:21 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 03:14:23 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Tue, 30 Nov 2021 03:14:23 GMT
WORKDIR /usr/local/apache2
# Tue, 30 Nov 2021 03:14:29 GMT
RUN set -eux; 	apk add --no-cache 		apr 		apr-util 		apr-util-ldap 		perl 	;
# Mon, 14 Mar 2022 18:24:11 GMT
ENV HTTPD_VERSION=2.4.53
# Mon, 14 Mar 2022 18:24:11 GMT
ENV HTTPD_SHA256=d0bbd1121a57b5f2a6ff92d7b96f8050c5a45d3f14db118f64979d525858db63
# Mon, 14 Mar 2022 18:24:12 GMT
ENV HTTPD_PATCHES=
# Mon, 14 Mar 2022 18:30:19 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		apr-dev 		apr-util-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://downloads.apache.org/ 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		DE29FB3971E71543FD2DC049508EAEC5302DA568 		13155B0E9E634F42BF6C163FDDBA64BA2C312D2F 		8B39757B1D8A994DF2433ED58B3A601F08C975E5 		31EE1A81B8D066548156D37B7D6DBFD1F08E012A 		A10208FEC3152DD7C0C9B59B361522D782AB7BD1 		3DE024AFDA7A4B15CB6C14410F81AA8AB0D5F771 		EB138C6AF0FC691001B16D93344A844D751D7F27 		CBA5A7C21EC143314C41393E5B968010E04F9A89 		3C016F2B764621BB549C66B516A96495E2226795 		937FB3994A242BA9BF49E93021454AF0CC8B0F7E 		EAD1359A4C0F2D37472AAF28F55DF0293A4E7AC9 		4C1EADADB4EF5007579C919C6635B6C0DE885DD3 		01E475360FCCF1D0F24B9D145D414AE1E005C9CB 		92CCEF0AA7DD46AC3A0F498BCA6939748103A37E 		D395C7573A68B9796D38C258153FA0CD75A67692 		FA39B617B61493FD283503E7EED1EA392261D073 		984FB3350C1D5C7A3282255BB31B213D208F5064 		FE7A49DAA875E890B4167F76CCB2EB46E76CF6D0 		39F6691A0ECF0C50E8BB849CF78875F642721F00 		29A2BA848177B73878277FA475CAA2A3F39B3750 		120A8667241AEDD4A78B46104C042818311A3DE5 		453510BDA6C5855624E009236D0BC73A40581837 		0DE5C55C6BF3B2352DABB89E13249B4FEC88A0BF 		7CDBED100806552182F98844E8E7E00B4DAA1988 		A8BA9617EF3BCCAC3B29B869EDB105896F9522D8 		3E6AC004854F3A7F03566B592FF06894E55B0D0E 		5B5181C2C0AB13E59DA3F7A3EC582EB639FF092C 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		65B2D44FE74BD5E3DE3AC3F082781DE46D5954FA 		8935926745E1CE7E3ED748F6EC99EE267EB5F61A 		E3480043595621FE56105F112AB12A7ADC55C003 		93525CFCF6FDFFB3FD9700DD5A4B10AE43B56A27 		C55AB7B9139EB2263CD1AABC19B033D1760C227B 		26F51EF9A82F4ACB43F1903ED377C9E7D1944C66 	; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*User)\s+daemon\s*$!\1 www-data!g' 		-e 's!^(\s*Group)\s+daemon\s*$!\1 www-data!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 	grep -E '^\s*User www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 	grep -E '^\s*Group www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 		deps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-so-deps $deps; 	apk del --no-network .build-deps; 		httpd -v
# Mon, 14 Mar 2022 18:30:19 GMT
STOPSIGNAL SIGWINCH
# Mon, 14 Mar 2022 18:30:20 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Mon, 14 Mar 2022 18:30:20 GMT
EXPOSE 80
# Mon, 14 Mar 2022 18:30:21 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:e4a43de54da9e309482f6762f0c11f5f547cd8fd61a49c5f158453066162023e`  
		Last Modified: Wed, 24 Nov 2021 21:09:46 GMT  
		Size: 2.6 MB (2631421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c4e7cc6c6a5c36d1bb79e27acfb9c33840791f6c0f0a982c03faf4ae8c20d3a1`  
		Last Modified: Tue, 30 Nov 2021 03:18:33 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5aef5164a7912b8708585f8f7c4946765f75e57430f36fc8ef99f4d1e04542c`  
		Last Modified: Tue, 30 Nov 2021 03:18:33 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008f53e39c8c35d1a942f1854f9710113e9aca04c9e14d833fac1ffcef2e5a8a`  
		Last Modified: Tue, 30 Nov 2021 03:18:40 GMT  
		Size: 8.7 MB (8747030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea574dd2ceb9d235b4e7e1712df81d765a58cefa41799b29e870c2fc75cefb7d`  
		Last Modified: Mon, 14 Mar 2022 18:31:17 GMT  
		Size: 5.6 MB (5599372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db05fb8051b70075d6ec5e89be7a1b3f3dc12dd3d5cacfdf7205e34210f58459`  
		Last Modified: Mon, 14 Mar 2022 18:31:13 GMT  
		Size: 300.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; arm variant v7

```console
$ docker pull httpd@sha256:356c40d85334d1030d3e205b7c533347f550bb4a6048afd9d33380cbdf41aece
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **16.2 MB (16210186 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:94b2496f40bb84a015a1efc8fa512f66a0baf5a7644bbcb3d57fd21ea47c5e82`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Wed, 24 Nov 2021 21:42:11 GMT
ADD file:ca436da5b0bfc9c0e2fc685533c6628918000c8fff109fe9a8da625b9a798002 in / 
# Wed, 24 Nov 2021 21:42:11 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 03:19:29 GMT
RUN set -x 	&& adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 03:19:29 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Tue, 30 Nov 2021 03:19:30 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 03:19:31 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Tue, 30 Nov 2021 03:19:32 GMT
WORKDIR /usr/local/apache2
# Tue, 30 Nov 2021 03:19:37 GMT
RUN set -eux; 	apk add --no-cache 		apr 		apr-util 		apr-util-ldap 		perl 	;
# Mon, 14 Mar 2022 19:38:42 GMT
ENV HTTPD_VERSION=2.4.53
# Mon, 14 Mar 2022 19:38:43 GMT
ENV HTTPD_SHA256=d0bbd1121a57b5f2a6ff92d7b96f8050c5a45d3f14db118f64979d525858db63
# Mon, 14 Mar 2022 19:38:43 GMT
ENV HTTPD_PATCHES=
# Mon, 14 Mar 2022 19:43:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		apr-dev 		apr-util-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://downloads.apache.org/ 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		DE29FB3971E71543FD2DC049508EAEC5302DA568 		13155B0E9E634F42BF6C163FDDBA64BA2C312D2F 		8B39757B1D8A994DF2433ED58B3A601F08C975E5 		31EE1A81B8D066548156D37B7D6DBFD1F08E012A 		A10208FEC3152DD7C0C9B59B361522D782AB7BD1 		3DE024AFDA7A4B15CB6C14410F81AA8AB0D5F771 		EB138C6AF0FC691001B16D93344A844D751D7F27 		CBA5A7C21EC143314C41393E5B968010E04F9A89 		3C016F2B764621BB549C66B516A96495E2226795 		937FB3994A242BA9BF49E93021454AF0CC8B0F7E 		EAD1359A4C0F2D37472AAF28F55DF0293A4E7AC9 		4C1EADADB4EF5007579C919C6635B6C0DE885DD3 		01E475360FCCF1D0F24B9D145D414AE1E005C9CB 		92CCEF0AA7DD46AC3A0F498BCA6939748103A37E 		D395C7573A68B9796D38C258153FA0CD75A67692 		FA39B617B61493FD283503E7EED1EA392261D073 		984FB3350C1D5C7A3282255BB31B213D208F5064 		FE7A49DAA875E890B4167F76CCB2EB46E76CF6D0 		39F6691A0ECF0C50E8BB849CF78875F642721F00 		29A2BA848177B73878277FA475CAA2A3F39B3750 		120A8667241AEDD4A78B46104C042818311A3DE5 		453510BDA6C5855624E009236D0BC73A40581837 		0DE5C55C6BF3B2352DABB89E13249B4FEC88A0BF 		7CDBED100806552182F98844E8E7E00B4DAA1988 		A8BA9617EF3BCCAC3B29B869EDB105896F9522D8 		3E6AC004854F3A7F03566B592FF06894E55B0D0E 		5B5181C2C0AB13E59DA3F7A3EC582EB639FF092C 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		65B2D44FE74BD5E3DE3AC3F082781DE46D5954FA 		8935926745E1CE7E3ED748F6EC99EE267EB5F61A 		E3480043595621FE56105F112AB12A7ADC55C003 		93525CFCF6FDFFB3FD9700DD5A4B10AE43B56A27 		C55AB7B9139EB2263CD1AABC19B033D1760C227B 		26F51EF9A82F4ACB43F1903ED377C9E7D1944C66 	; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*User)\s+daemon\s*$!\1 www-data!g' 		-e 's!^(\s*Group)\s+daemon\s*$!\1 www-data!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 	grep -E '^\s*User www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 	grep -E '^\s*Group www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 		deps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-so-deps $deps; 	apk del --no-network .build-deps; 		httpd -v
# Mon, 14 Mar 2022 19:43:24 GMT
STOPSIGNAL SIGWINCH
# Mon, 14 Mar 2022 19:43:25 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Mon, 14 Mar 2022 19:43:25 GMT
EXPOSE 80
# Mon, 14 Mar 2022 19:43:25 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:5480d2ca1740c20ce17652e01ed2265cdc914458acd41256a2b1ccff28f2762c`  
		Last Modified: Wed, 24 Nov 2021 21:43:40 GMT  
		Size: 2.4 MB (2434764 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dfdb7342e218dc38386e9ff7f2fd20cdd6896e2e8c6d331cf3b21d33b47dd58`  
		Last Modified: Tue, 30 Nov 2021 03:23:48 GMT  
		Size: 1.3 KB (1255 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe679c702b5b8004f6d352b0948e6bf860afabdb25fcb401bf5603ec1ff19695`  
		Last Modified: Tue, 30 Nov 2021 03:23:48 GMT  
		Size: 177.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bcdee90c1c8660881f5e8e35e0e3457cb76265581bfff10bf3825da8a9fda160`  
		Last Modified: Tue, 30 Nov 2021 03:23:56 GMT  
		Size: 8.5 MB (8535355 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc22f4cb8759b3d924ab3d8e362b69ab33a5b194b62fd92e31235f9251e55e81`  
		Last Modified: Mon, 14 Mar 2022 19:45:42 GMT  
		Size: 5.2 MB (5238335 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66706ea4273334dc06594e17f9a07419e89ac53ecd9f8ad07359206c8542c822`  
		Last Modified: Mon, 14 Mar 2022 19:45:38 GMT  
		Size: 300.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; arm64 variant v8

```console
$ docker pull httpd@sha256:b91fa7dd0b5cb4da2d2fea87039bbde8731016a1acca35b001e7210a5504287c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 MB (17905301 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31b769b59a5136ec9ba693d82cb9d8f832acaeeef94b1e35d35306707369ece5`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Wed, 24 Nov 2021 20:39:20 GMT
ADD file:df53811312284306901fdaaff0a357a4bf40d631e662fe9ce6d342442e494b6c in / 
# Wed, 24 Nov 2021 20:39:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 02:13:42 GMT
RUN set -x 	&& adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 02:13:43 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Tue, 30 Nov 2021 02:13:44 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 02:13:45 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Tue, 30 Nov 2021 02:13:46 GMT
WORKDIR /usr/local/apache2
# Tue, 30 Nov 2021 02:13:48 GMT
RUN set -eux; 	apk add --no-cache 		apr 		apr-util 		apr-util-ldap 		perl 	;
# Mon, 14 Mar 2022 18:35:32 GMT
ENV HTTPD_VERSION=2.4.53
# Mon, 14 Mar 2022 18:35:33 GMT
ENV HTTPD_SHA256=d0bbd1121a57b5f2a6ff92d7b96f8050c5a45d3f14db118f64979d525858db63
# Mon, 14 Mar 2022 18:35:34 GMT
ENV HTTPD_PATCHES=
# Mon, 14 Mar 2022 18:38:50 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		apr-dev 		apr-util-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://downloads.apache.org/ 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		DE29FB3971E71543FD2DC049508EAEC5302DA568 		13155B0E9E634F42BF6C163FDDBA64BA2C312D2F 		8B39757B1D8A994DF2433ED58B3A601F08C975E5 		31EE1A81B8D066548156D37B7D6DBFD1F08E012A 		A10208FEC3152DD7C0C9B59B361522D782AB7BD1 		3DE024AFDA7A4B15CB6C14410F81AA8AB0D5F771 		EB138C6AF0FC691001B16D93344A844D751D7F27 		CBA5A7C21EC143314C41393E5B968010E04F9A89 		3C016F2B764621BB549C66B516A96495E2226795 		937FB3994A242BA9BF49E93021454AF0CC8B0F7E 		EAD1359A4C0F2D37472AAF28F55DF0293A4E7AC9 		4C1EADADB4EF5007579C919C6635B6C0DE885DD3 		01E475360FCCF1D0F24B9D145D414AE1E005C9CB 		92CCEF0AA7DD46AC3A0F498BCA6939748103A37E 		D395C7573A68B9796D38C258153FA0CD75A67692 		FA39B617B61493FD283503E7EED1EA392261D073 		984FB3350C1D5C7A3282255BB31B213D208F5064 		FE7A49DAA875E890B4167F76CCB2EB46E76CF6D0 		39F6691A0ECF0C50E8BB849CF78875F642721F00 		29A2BA848177B73878277FA475CAA2A3F39B3750 		120A8667241AEDD4A78B46104C042818311A3DE5 		453510BDA6C5855624E009236D0BC73A40581837 		0DE5C55C6BF3B2352DABB89E13249B4FEC88A0BF 		7CDBED100806552182F98844E8E7E00B4DAA1988 		A8BA9617EF3BCCAC3B29B869EDB105896F9522D8 		3E6AC004854F3A7F03566B592FF06894E55B0D0E 		5B5181C2C0AB13E59DA3F7A3EC582EB639FF092C 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		65B2D44FE74BD5E3DE3AC3F082781DE46D5954FA 		8935926745E1CE7E3ED748F6EC99EE267EB5F61A 		E3480043595621FE56105F112AB12A7ADC55C003 		93525CFCF6FDFFB3FD9700DD5A4B10AE43B56A27 		C55AB7B9139EB2263CD1AABC19B033D1760C227B 		26F51EF9A82F4ACB43F1903ED377C9E7D1944C66 	; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*User)\s+daemon\s*$!\1 www-data!g' 		-e 's!^(\s*Group)\s+daemon\s*$!\1 www-data!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 	grep -E '^\s*User www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 	grep -E '^\s*Group www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 		deps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-so-deps $deps; 	apk del --no-network .build-deps; 		httpd -v
# Mon, 14 Mar 2022 18:38:51 GMT
STOPSIGNAL SIGWINCH
# Mon, 14 Mar 2022 18:38:53 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Mon, 14 Mar 2022 18:38:53 GMT
EXPOSE 80
# Mon, 14 Mar 2022 18:38:54 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:9b3977197b4f2147bdd31e1271f811319dcd5c2fc595f14e81f5351ab6275b99`  
		Last Modified: Wed, 24 Nov 2021 20:39:59 GMT  
		Size: 2.7 MB (2715434 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d9e1f41284186a13b72b5c042b733c4e211d6dc47532ccc08a158e2480bc02a`  
		Last Modified: Tue, 30 Nov 2021 02:16:14 GMT  
		Size: 1.2 KB (1233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55c32d614302454d100dbc031565bcde98b4617dd2f4f93aa70178574b03c90e`  
		Last Modified: Tue, 30 Nov 2021 02:16:14 GMT  
		Size: 147.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f09380cbcdb798ac55e14b28c2168e5b4aed7bb65b605d76695a8cd1453d6460`  
		Last Modified: Tue, 30 Nov 2021 02:16:16 GMT  
		Size: 9.5 MB (9510774 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0d25322afde91122f365beb0d2f6bca93b735816998c5c9de27067ac71d66062`  
		Last Modified: Mon, 14 Mar 2022 18:40:06 GMT  
		Size: 5.7 MB (5677415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:20969fa15e57c3dc3faa37f64316847ec1cbbf098ff45f1dbcc721a714b0e7c0`  
		Last Modified: Mon, 14 Mar 2022 18:40:04 GMT  
		Size: 298.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; 386

```console
$ docker pull httpd@sha256:dbe56c6cd7ef868e3853d3dfc75fc00b0100096dc852ebc18f8dc1c11210f1e1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 MB (17717218 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f5db3539f2a339993ce2eeb4574bd68192aeafabbc200b07768da33bd4332865`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Wed, 24 Nov 2021 20:53:48 GMT
ADD file:b9a17131c440053f2f67e127b447645f25fd7de2d6caca42f569cafab6291855 in / 
# Wed, 24 Nov 2021 20:53:48 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 02:18:00 GMT
RUN set -x 	&& adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 02:18:00 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Tue, 30 Nov 2021 02:18:00 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 02:18:01 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Tue, 30 Nov 2021 02:18:01 GMT
WORKDIR /usr/local/apache2
# Tue, 30 Nov 2021 02:18:04 GMT
RUN set -eux; 	apk add --no-cache 		apr 		apr-util 		apr-util-ldap 		perl 	;
# Mon, 14 Mar 2022 19:55:05 GMT
ENV HTTPD_VERSION=2.4.53
# Mon, 14 Mar 2022 19:55:05 GMT
ENV HTTPD_SHA256=d0bbd1121a57b5f2a6ff92d7b96f8050c5a45d3f14db118f64979d525858db63
# Mon, 14 Mar 2022 19:55:05 GMT
ENV HTTPD_PATCHES=
# Mon, 14 Mar 2022 19:57:36 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		apr-dev 		apr-util-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://downloads.apache.org/ 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		DE29FB3971E71543FD2DC049508EAEC5302DA568 		13155B0E9E634F42BF6C163FDDBA64BA2C312D2F 		8B39757B1D8A994DF2433ED58B3A601F08C975E5 		31EE1A81B8D066548156D37B7D6DBFD1F08E012A 		A10208FEC3152DD7C0C9B59B361522D782AB7BD1 		3DE024AFDA7A4B15CB6C14410F81AA8AB0D5F771 		EB138C6AF0FC691001B16D93344A844D751D7F27 		CBA5A7C21EC143314C41393E5B968010E04F9A89 		3C016F2B764621BB549C66B516A96495E2226795 		937FB3994A242BA9BF49E93021454AF0CC8B0F7E 		EAD1359A4C0F2D37472AAF28F55DF0293A4E7AC9 		4C1EADADB4EF5007579C919C6635B6C0DE885DD3 		01E475360FCCF1D0F24B9D145D414AE1E005C9CB 		92CCEF0AA7DD46AC3A0F498BCA6939748103A37E 		D395C7573A68B9796D38C258153FA0CD75A67692 		FA39B617B61493FD283503E7EED1EA392261D073 		984FB3350C1D5C7A3282255BB31B213D208F5064 		FE7A49DAA875E890B4167F76CCB2EB46E76CF6D0 		39F6691A0ECF0C50E8BB849CF78875F642721F00 		29A2BA848177B73878277FA475CAA2A3F39B3750 		120A8667241AEDD4A78B46104C042818311A3DE5 		453510BDA6C5855624E009236D0BC73A40581837 		0DE5C55C6BF3B2352DABB89E13249B4FEC88A0BF 		7CDBED100806552182F98844E8E7E00B4DAA1988 		A8BA9617EF3BCCAC3B29B869EDB105896F9522D8 		3E6AC004854F3A7F03566B592FF06894E55B0D0E 		5B5181C2C0AB13E59DA3F7A3EC582EB639FF092C 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		65B2D44FE74BD5E3DE3AC3F082781DE46D5954FA 		8935926745E1CE7E3ED748F6EC99EE267EB5F61A 		E3480043595621FE56105F112AB12A7ADC55C003 		93525CFCF6FDFFB3FD9700DD5A4B10AE43B56A27 		C55AB7B9139EB2263CD1AABC19B033D1760C227B 		26F51EF9A82F4ACB43F1903ED377C9E7D1944C66 	; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*User)\s+daemon\s*$!\1 www-data!g' 		-e 's!^(\s*Group)\s+daemon\s*$!\1 www-data!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 	grep -E '^\s*User www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 	grep -E '^\s*Group www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 		deps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-so-deps $deps; 	apk del --no-network .build-deps; 		httpd -v
# Mon, 14 Mar 2022 19:57:36 GMT
STOPSIGNAL SIGWINCH
# Mon, 14 Mar 2022 19:57:36 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Mon, 14 Mar 2022 19:57:36 GMT
EXPOSE 80
# Mon, 14 Mar 2022 19:57:37 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:e6889e0d66307a4b916fc844f2dcbc03245c63bc4189dd3e88126d9dcf2f9231`  
		Last Modified: Wed, 24 Nov 2021 20:54:48 GMT  
		Size: 2.8 MB (2827117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a723b4523b798c534842c3a17b74cdf76ea290b6dfa4f812af0b2f31fa16369d`  
		Last Modified: Tue, 30 Nov 2021 02:21:37 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7080df26ee2a949ca98ed523c8fbfd34802ef9f7e6f818681c9e665f10f8004`  
		Last Modified: Tue, 30 Nov 2021 02:21:37 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:72e1e4b5af942db6fa58488a1294760ec45ab81c6f720b81fc777e4fb785a403`  
		Last Modified: Tue, 30 Nov 2021 02:21:40 GMT  
		Size: 8.9 MB (8945942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0a0f0e7864845b71ec05dae1665d8ef005d241bc267b8a8a38a33173f2dac4b`  
		Last Modified: Mon, 14 Mar 2022 19:59:02 GMT  
		Size: 5.9 MB (5942425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:158ab79b164ecbbee75724abb204588a3cafdb5ae2c5fe561606f5548a1aa9b4`  
		Last Modified: Mon, 14 Mar 2022 19:59:00 GMT  
		Size: 300.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; ppc64le

```console
$ docker pull httpd@sha256:e0b631f4e920a1d037c9b5f3944ad5286bbd0a15863b2a2cc07b9e5e9c6daa42
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 MB (18598061 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffee8a24e89d09647e1cdcae7e589f77eff06bb5b71d53d28c1deeae22d5cc53`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Wed, 24 Nov 2021 20:20:16 GMT
ADD file:57115dca2eb707f46b6301e75174e6aa316fb02ac28643b91429b75be51bd8c8 in / 
# Wed, 24 Nov 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:18:07 GMT
RUN set -x 	&& adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 04:18:12 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Tue, 30 Nov 2021 04:18:13 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 04:18:20 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Tue, 30 Nov 2021 04:18:23 GMT
WORKDIR /usr/local/apache2
# Tue, 30 Nov 2021 04:18:32 GMT
RUN set -eux; 	apk add --no-cache 		apr 		apr-util 		apr-util-ldap 		perl 	;
# Mon, 14 Mar 2022 21:11:30 GMT
ENV HTTPD_VERSION=2.4.53
# Mon, 14 Mar 2022 21:11:35 GMT
ENV HTTPD_SHA256=d0bbd1121a57b5f2a6ff92d7b96f8050c5a45d3f14db118f64979d525858db63
# Mon, 14 Mar 2022 21:11:38 GMT
ENV HTTPD_PATCHES=
# Mon, 14 Mar 2022 21:17:26 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		apr-dev 		apr-util-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://downloads.apache.org/ 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		DE29FB3971E71543FD2DC049508EAEC5302DA568 		13155B0E9E634F42BF6C163FDDBA64BA2C312D2F 		8B39757B1D8A994DF2433ED58B3A601F08C975E5 		31EE1A81B8D066548156D37B7D6DBFD1F08E012A 		A10208FEC3152DD7C0C9B59B361522D782AB7BD1 		3DE024AFDA7A4B15CB6C14410F81AA8AB0D5F771 		EB138C6AF0FC691001B16D93344A844D751D7F27 		CBA5A7C21EC143314C41393E5B968010E04F9A89 		3C016F2B764621BB549C66B516A96495E2226795 		937FB3994A242BA9BF49E93021454AF0CC8B0F7E 		EAD1359A4C0F2D37472AAF28F55DF0293A4E7AC9 		4C1EADADB4EF5007579C919C6635B6C0DE885DD3 		01E475360FCCF1D0F24B9D145D414AE1E005C9CB 		92CCEF0AA7DD46AC3A0F498BCA6939748103A37E 		D395C7573A68B9796D38C258153FA0CD75A67692 		FA39B617B61493FD283503E7EED1EA392261D073 		984FB3350C1D5C7A3282255BB31B213D208F5064 		FE7A49DAA875E890B4167F76CCB2EB46E76CF6D0 		39F6691A0ECF0C50E8BB849CF78875F642721F00 		29A2BA848177B73878277FA475CAA2A3F39B3750 		120A8667241AEDD4A78B46104C042818311A3DE5 		453510BDA6C5855624E009236D0BC73A40581837 		0DE5C55C6BF3B2352DABB89E13249B4FEC88A0BF 		7CDBED100806552182F98844E8E7E00B4DAA1988 		A8BA9617EF3BCCAC3B29B869EDB105896F9522D8 		3E6AC004854F3A7F03566B592FF06894E55B0D0E 		5B5181C2C0AB13E59DA3F7A3EC582EB639FF092C 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		65B2D44FE74BD5E3DE3AC3F082781DE46D5954FA 		8935926745E1CE7E3ED748F6EC99EE267EB5F61A 		E3480043595621FE56105F112AB12A7ADC55C003 		93525CFCF6FDFFB3FD9700DD5A4B10AE43B56A27 		C55AB7B9139EB2263CD1AABC19B033D1760C227B 		26F51EF9A82F4ACB43F1903ED377C9E7D1944C66 	; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*User)\s+daemon\s*$!\1 www-data!g' 		-e 's!^(\s*Group)\s+daemon\s*$!\1 www-data!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 	grep -E '^\s*User www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 	grep -E '^\s*Group www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 		deps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-so-deps $deps; 	apk del --no-network .build-deps; 		httpd -v
# Mon, 14 Mar 2022 21:17:30 GMT
STOPSIGNAL SIGWINCH
# Mon, 14 Mar 2022 21:17:32 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Mon, 14 Mar 2022 21:17:36 GMT
EXPOSE 80
# Mon, 14 Mar 2022 21:17:39 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:159b5dcb1717c815c76ff5ea1db730e18e8609c9090238e43282856db9e71f47`  
		Last Modified: Wed, 24 Nov 2021 20:21:14 GMT  
		Size: 2.8 MB (2814780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:707368fa235e16293c35f77f1b9389c8c2535546860d2fd7b1089af914f15b60`  
		Last Modified: Tue, 30 Nov 2021 04:21:34 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0732cee0c651c0756e32bd4bbc47f4265b027fdb0e6d5cd5e177f2eb0920e012`  
		Last Modified: Tue, 30 Nov 2021 04:21:34 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cda6f1cf7a48f950375ff7cfbfeee668656a16e5b7f77a4fc348ef9838fcb943`  
		Last Modified: Tue, 30 Nov 2021 04:21:39 GMT  
		Size: 9.6 MB (9649735 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e54199ce3902714e4db8d6a84223068b86bfccd97b7479edfa4fc575600d781d`  
		Last Modified: Mon, 14 Mar 2022 21:19:19 GMT  
		Size: 6.1 MB (6131806 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2a7e9156918cb2843f84f028af19182f3ac924d28baa2822074032153f03955c`  
		Last Modified: Mon, 14 Mar 2022 21:19:13 GMT  
		Size: 301.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `httpd:2-alpine` - linux; s390x

```console
$ docker pull httpd@sha256:2886bf4bea49ec3e6404ea85b1feea2a9045bf035cf29bc392dee5109269b8b3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.3 MB (18314990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:291e46f8734c96041608220bec9934b7e4703248b89cc7960ac0d08b8cd73cb8`
-	Default Command: `["httpd-foreground"]`

```dockerfile
# Wed, 24 Nov 2021 20:41:23 GMT
ADD file:cd24c711a2ef431b3ff94f9a02bfc42f159bc60de1d0eceecafea4e8af02441d in / 
# Wed, 24 Nov 2021 20:41:23 GMT
CMD ["/bin/sh"]
# Tue, 30 Nov 2021 04:20:42 GMT
RUN set -x 	&& adduser -u 82 -D -S -G www-data www-data
# Tue, 30 Nov 2021 04:20:42 GMT
ENV HTTPD_PREFIX=/usr/local/apache2
# Tue, 30 Nov 2021 04:20:42 GMT
ENV PATH=/usr/local/apache2/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Nov 2021 04:20:43 GMT
RUN mkdir -p "$HTTPD_PREFIX" 	&& chown www-data:www-data "$HTTPD_PREFIX"
# Tue, 30 Nov 2021 04:20:43 GMT
WORKDIR /usr/local/apache2
# Tue, 30 Nov 2021 04:20:45 GMT
RUN set -eux; 	apk add --no-cache 		apr 		apr-util 		apr-util-ldap 		perl 	;
# Mon, 14 Mar 2022 18:31:08 GMT
ENV HTTPD_VERSION=2.4.53
# Mon, 14 Mar 2022 18:31:09 GMT
ENV HTTPD_SHA256=d0bbd1121a57b5f2a6ff92d7b96f8050c5a45d3f14db118f64979d525858db63
# Mon, 14 Mar 2022 18:31:09 GMT
ENV HTTPD_PATCHES=
# Mon, 14 Mar 2022 18:36:32 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		apr-dev 		apr-util-dev 		ca-certificates 		coreutils 		dpkg-dev dpkg 		gcc 		gnupg 		libc-dev 		curl-dev 		jansson-dev 		libxml2-dev 		lua-dev 		make 		nghttp2-dev 		openssl 		openssl-dev 		pcre-dev 		tar 		zlib-dev 		brotli-dev 	; 		ddist() { 		local f="$1"; shift; 		local distFile="$1"; shift; 		local success=; 		local distUrl=; 		for distUrl in 			'https://www.apache.org/dyn/closer.cgi?action=download&filename=' 			https://downloads.apache.org/ 			https://www-us.apache.org/dist/ 			https://www.apache.org/dist/ 			https://archive.apache.org/dist/ 		; do 			if wget -O "$f" "$distUrl$distFile" && [ -s "$f" ]; then 				success=1; 				break; 			fi; 		done; 		[ -n "$success" ]; 	}; 		ddist 'httpd.tar.bz2' "httpd/httpd-$HTTPD_VERSION.tar.bz2"; 	echo "$HTTPD_SHA256 *httpd.tar.bz2" | sha256sum -c -; 		ddist 'httpd.tar.bz2.asc' "httpd/httpd-$HTTPD_VERSION.tar.bz2.asc"; 	export GNUPGHOME="$(mktemp -d)"; 	for key in 		DE29FB3971E71543FD2DC049508EAEC5302DA568 		13155B0E9E634F42BF6C163FDDBA64BA2C312D2F 		8B39757B1D8A994DF2433ED58B3A601F08C975E5 		31EE1A81B8D066548156D37B7D6DBFD1F08E012A 		A10208FEC3152DD7C0C9B59B361522D782AB7BD1 		3DE024AFDA7A4B15CB6C14410F81AA8AB0D5F771 		EB138C6AF0FC691001B16D93344A844D751D7F27 		CBA5A7C21EC143314C41393E5B968010E04F9A89 		3C016F2B764621BB549C66B516A96495E2226795 		937FB3994A242BA9BF49E93021454AF0CC8B0F7E 		EAD1359A4C0F2D37472AAF28F55DF0293A4E7AC9 		4C1EADADB4EF5007579C919C6635B6C0DE885DD3 		01E475360FCCF1D0F24B9D145D414AE1E005C9CB 		92CCEF0AA7DD46AC3A0F498BCA6939748103A37E 		D395C7573A68B9796D38C258153FA0CD75A67692 		FA39B617B61493FD283503E7EED1EA392261D073 		984FB3350C1D5C7A3282255BB31B213D208F5064 		FE7A49DAA875E890B4167F76CCB2EB46E76CF6D0 		39F6691A0ECF0C50E8BB849CF78875F642721F00 		29A2BA848177B73878277FA475CAA2A3F39B3750 		120A8667241AEDD4A78B46104C042818311A3DE5 		453510BDA6C5855624E009236D0BC73A40581837 		0DE5C55C6BF3B2352DABB89E13249B4FEC88A0BF 		7CDBED100806552182F98844E8E7E00B4DAA1988 		A8BA9617EF3BCCAC3B29B869EDB105896F9522D8 		3E6AC004854F3A7F03566B592FF06894E55B0D0E 		5B5181C2C0AB13E59DA3F7A3EC582EB639FF092C 		A93D62ECC3C8EA12DB220EC934EA76E6791485A8 		65B2D44FE74BD5E3DE3AC3F082781DE46D5954FA 		8935926745E1CE7E3ED748F6EC99EE267EB5F61A 		E3480043595621FE56105F112AB12A7ADC55C003 		93525CFCF6FDFFB3FD9700DD5A4B10AE43B56A27 		C55AB7B9139EB2263CD1AABC19B033D1760C227B 		26F51EF9A82F4ACB43F1903ED377C9E7D1944C66 	; do 		gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$key"; 	done; 	gpg --batch --verify httpd.tar.bz2.asc httpd.tar.bz2; 	command -v gpgconf && gpgconf --kill all || :; 	rm -rf "$GNUPGHOME" httpd.tar.bz2.asc; 		mkdir -p src; 	tar -xf httpd.tar.bz2 -C src --strip-components=1; 	rm httpd.tar.bz2; 	cd src; 		patches() { 		while [ "$#" -gt 0 ]; do 			local patchFile="$1"; shift; 			local patchSha256="$1"; shift; 			ddist "$patchFile" "httpd/patches/apply_to_$HTTPD_VERSION/$patchFile"; 			echo "$patchSha256 *$patchFile" | sha256sum -c -; 			patch -p0 < "$patchFile"; 			rm -f "$patchFile"; 		done; 	}; 	patches $HTTPD_PATCHES; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--prefix="$HTTPD_PREFIX" 		--enable-mods-shared=reallyall 		--enable-mpms-shared=all 	; 	make -j "$(nproc)"; 	make install; 		cd ..; 	rm -r src man manual; 		sed -ri 		-e 's!^(\s*CustomLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*ErrorLog)\s+\S+!\1 /proc/self/fd/2!g' 		-e 's!^(\s*TransferLog)\s+\S+!\1 /proc/self/fd/1!g' 		-e 's!^(\s*User)\s+daemon\s*$!\1 www-data!g' 		-e 's!^(\s*Group)\s+daemon\s*$!\1 www-data!g' 		"$HTTPD_PREFIX/conf/httpd.conf" 		"$HTTPD_PREFIX/conf/extra/httpd-ssl.conf" 	; 	grep -E '^\s*User www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 	grep -E '^\s*Group www-data$' "$HTTPD_PREFIX/conf/httpd.conf"; 		deps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .httpd-so-deps $deps; 	apk del --no-network .build-deps; 		httpd -v
# Mon, 14 Mar 2022 18:36:32 GMT
STOPSIGNAL SIGWINCH
# Mon, 14 Mar 2022 18:36:32 GMT
COPY file:c432ff61c4993ecdef4786f48d91a96f8f0707f6179816ccb98db661bfb96b90 in /usr/local/bin/ 
# Mon, 14 Mar 2022 18:36:32 GMT
EXPOSE 80
# Mon, 14 Mar 2022 18:36:32 GMT
CMD ["httpd-foreground"]
```

-	Layers:
	-	`sha256:d6baca485f3d0f7c77221be60fbef5db014a5ef9d8f53db4a310c947c690d189`  
		Last Modified: Wed, 24 Nov 2021 20:42:15 GMT  
		Size: 2.6 MB (2605944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4420734ecc329e8e35fe109761729d10c6237e043dfc073bf4f84533a33e0f`  
		Last Modified: Tue, 30 Nov 2021 04:23:08 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0544c352d66a74f15db1ee1f9bd04a46ea2301638f67b3554166d4fe319c31`  
		Last Modified: Tue, 30 Nov 2021 04:23:08 GMT  
		Size: 178.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7bcdf1566943622d80ba64f883d8dd41e6a6c721bf41ae86fc8c23714d07fe95`  
		Last Modified: Tue, 30 Nov 2021 04:23:10 GMT  
		Size: 10.0 MB (9986098 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2474d9edee819cd34e86d3598aaa94c972e749639f6a768587fc74ceb8e2947`  
		Last Modified: Mon, 14 Mar 2022 18:37:40 GMT  
		Size: 5.7 MB (5721213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f7aeeceed75d93dfc566f1876848a9347129560f0cd1231518a5a709ee74e07`  
		Last Modified: Mon, 14 Mar 2022 18:37:40 GMT  
		Size: 298.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
