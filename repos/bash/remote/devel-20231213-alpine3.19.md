## `bash:devel-20231213-alpine3.19`

```console
$ docker pull bash@sha256:13df6b45f8e647db4d186b0198459cd295b3bc61de29db4a7fc5bb5944ec1396
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; arm variant v6

### `bash:devel-20231213-alpine3.19` - linux; arm variant v6

```console
$ docker pull bash@sha256:e37b6fa1ea502973e1629e75ea4bd978f460d1ca2d4ef4d147937a28f7225b90
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5971020 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bcd15cb3fcf75f724ba3ab3305c0a5a97d80313a06e917a3e28c7c0343d5404b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Fri, 08 Dec 2023 01:49:15 GMT
ADD file:d43ed267a41631ce0e5a4ef5aac821a75300a83f85ecb6259f5616852f89e989 in / 
# Fri, 08 Dec 2023 01:49:15 GMT
CMD ["/bin/sh"]
# Tue, 19 Dec 2023 20:49:19 GMT
ENV _BASH_COMMIT=9d51df7546eab80ea6baa4a83b2ae2178e8020c5
# Tue, 19 Dec 2023 20:49:20 GMT
ENV _BASH_VERSION=devel-20231213
# Tue, 19 Dec 2023 20:50:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		patch 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		{ echo '#include <unistd.h>'; echo; cat /usr/src/bash/lib/sh/strscpy.c; } > /usr/src/bash/lib/sh/strscpy.c.new; 	mv /usr/src/bash/lib/sh/strscpy.c.new /usr/src/bash/lib/sh/strscpy.c; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Tue, 19 Dec 2023 20:50:37 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Tue, 19 Dec 2023 20:50:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 19 Dec 2023 20:50:38 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:0803c38384d9fd0f9afaec8fd13d267547b660dcd46bb92a3d63c5d76e78b04c`  
		Last Modified: Fri, 08 Dec 2023 01:49:33 GMT  
		Size: 3.2 MB (3165143 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:393adb64eeab200f05b8762a288f066ffe59065a4e2da431b2aa6b3885b0f484`  
		Last Modified: Tue, 19 Dec 2023 20:51:56 GMT  
		Size: 2.8 MB (2805537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da7fe33ad7df72175e1939d2ee5697d7aec4e993157fb59ac4b93847dbf0d10b`  
		Last Modified: Tue, 19 Dec 2023 20:51:56 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
