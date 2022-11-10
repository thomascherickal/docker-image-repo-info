## `bash:devel`

```console
$ docker pull bash@sha256:d16bba9fddf17cd95a9ed60a8b99cd7098d27ff47411bd405cefe80635cb5e71
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

### `bash:devel` - linux; amd64

```console
$ docker pull bash@sha256:e1773a3e8a029fefc62b74b6dcd41b47de1dc3b849a029fbbf79a3878bc8e4bf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (5991470 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee1e82e41c6011ee42b0fa18a4ea9e6da214c979d0ae60cf35cb84b91c6472a8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Aug 2022 17:19:53 GMT
ADD file:2a949686d9886ac7c10582a6c29116fd29d3077d02755e87e111870d63607725 in / 
# Tue, 09 Aug 2022 17:19:53 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 01:19:30 GMT
ENV _BASH_COMMIT=31f4d468b60eb27d768ef56d0a8b4982346465d9
# Thu, 10 Nov 2022 01:19:30 GMT
ENV _BASH_VERSION=devel-20221107
# Thu, 10 Nov 2022 01:20:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Thu, 10 Nov 2022 01:20:11 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 10 Nov 2022 01:20:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 01:20:11 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:213ec9aee27d8be045c6a92b7eac22c9a64b44558193775a1a7f626352392b49`  
		Last Modified: Tue, 09 Aug 2022 14:25:13 GMT  
		Size: 2.8 MB (2806054 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac95bd0900c0e0b8d24e56eeda46843710eefed1b4b57673eb13e3eabddbf4cd`  
		Last Modified: Thu, 10 Nov 2022 01:34:41 GMT  
		Size: 3.2 MB (3185076 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:722adb9e72c8e7e2c0d732b960db7fbac00496c86621c4d2f221c506d3b39c45`  
		Last Modified: Thu, 10 Nov 2022 01:34:41 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel` - linux; arm variant v6

```console
$ docker pull bash@sha256:18cdd56e334ff3592d5063e7a8e8f8162053ec2466a4139129819f5a9b7cd11f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 MB (5719611 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5c8f2a1c75cf10b040712892980586e7de86e2b5f3bbf72537d4c535433a8746`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Aug 2022 17:49:22 GMT
ADD file:e8733e8cc0a81e15ca4041760b6e27392c34171512d34405a9b262b1fff5c687 in / 
# Tue, 09 Aug 2022 17:49:22 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 00:49:24 GMT
ENV _BASH_COMMIT=31f4d468b60eb27d768ef56d0a8b4982346465d9
# Thu, 10 Nov 2022 00:49:24 GMT
ENV _BASH_VERSION=devel-20221107
# Thu, 10 Nov 2022 00:50:14 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Thu, 10 Nov 2022 00:50:14 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 10 Nov 2022 00:50:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 00:50:14 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9506b835437abb4d8ba1683e00c500b8f77e1975e930b356fbb72f2dbdc274d9`  
		Last Modified: Tue, 09 Aug 2022 17:50:33 GMT  
		Size: 2.6 MB (2613965 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99980fe64151709cbf415cd4543ccfb33d4d2ec9f9895df0d1687d3ceb1636d`  
		Last Modified: Thu, 10 Nov 2022 01:06:01 GMT  
		Size: 3.1 MB (3105303 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0e40c9f8a958ca9a234935c74661e17c0e8ca9c559aa852dd0a1d59f55e74c`  
		Last Modified: Thu, 10 Nov 2022 01:06:00 GMT  
		Size: 343.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel` - linux; arm variant v7

```console
$ docker pull bash@sha256:e6bae67a1ca1aaa6f6d76ba7affe30994d028468dd2d6abbde694f535838555f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1805b075ea7c9837e8cbc18257a851036bebe5168b343636a0bb91caadfba122`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Aug 2022 16:57:44 GMT
ADD file:75521fe16320b193092588f6f31052c85e736965ceb11673de18bd14965a45e6 in / 
# Tue, 09 Aug 2022 16:57:44 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 00:59:51 GMT
ENV _BASH_COMMIT=31f4d468b60eb27d768ef56d0a8b4982346465d9
# Thu, 10 Nov 2022 00:59:52 GMT
ENV _BASH_VERSION=devel-20221107
# Thu, 10 Nov 2022 01:00:41 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Thu, 10 Nov 2022 01:00:41 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 10 Nov 2022 01:00:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 01:00:41 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c6556b3b6858c6fa1e328377cc2c4becdc9cd1bc3e7302aa7299936522cf93ba`  
		Last Modified: Tue, 09 Aug 2022 16:58:55 GMT  
		Size: 2.4 MB (2417065 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b173050c645cc3f5387ae500191c5e3fc69dd41692da003a3b73574bfb9f4e4d`  
		Last Modified: Thu, 10 Nov 2022 01:17:36 GMT  
		Size: 3.0 MB (3027321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57d0a805fe12374a92811a3d73da0cee7f7c0d0994e8485495482086293a3340`  
		Last Modified: Thu, 10 Nov 2022 01:17:35 GMT  
		Size: 337.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel` - linux; arm64 variant v8

```console
$ docker pull bash@sha256:44ee7d90934420261948c7ec0179d9805d7ef6187d801f5b32e202a35573183c
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5900983 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4a9afaff6a8d7ba22aea420ffa9fde03660852f6838214db2b945aded9692bf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Aug 2022 17:39:41 GMT
ADD file:960fd469d48cf79ba14bbda71f3192074ed860c112e30e0bc92bff3440cb45ab in / 
# Tue, 09 Aug 2022 17:39:42 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 00:39:22 GMT
ENV _BASH_COMMIT=31f4d468b60eb27d768ef56d0a8b4982346465d9
# Thu, 10 Nov 2022 00:39:23 GMT
ENV _BASH_VERSION=devel-20221107
# Thu, 10 Nov 2022 00:39:57 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Thu, 10 Nov 2022 00:39:57 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 10 Nov 2022 00:39:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 00:39:57 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:9b18e9b68314027565b90ff6189d65942c0f7986da80df008b8431276885218e`  
		Last Modified: Tue, 09 Aug 2022 17:40:38 GMT  
		Size: 2.7 MB (2707663 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db3edfe1e59a488b7d8e1a8b31d635bcd3c38354ba6044bb6d902809e53cff73`  
		Last Modified: Thu, 10 Nov 2022 00:52:56 GMT  
		Size: 3.2 MB (3192985 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4eeb346e07d05ee541b356523c483040d6f0293b081e0ef63e84134cb5bbd59d`  
		Last Modified: Thu, 10 Nov 2022 00:52:56 GMT  
		Size: 335.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel` - linux; 386

```console
$ docker pull bash@sha256:c47dfaf38477b2e0c5f3ca7aa46f34ff2df9680db3f6b872d5b4bb469f9f05c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5938428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc154ed0d58eb1a23355cc5b82178f6c1c163afe4391bc4f4a3d20f383ab2e3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Aug 2022 17:38:39 GMT
ADD file:b828bc14bc5ff03c8f7310fe0aed6ac5df19a393622d5d1d779a523234d07c0a in / 
# Tue, 09 Aug 2022 17:38:39 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 00:38:26 GMT
ENV _BASH_COMMIT=31f4d468b60eb27d768ef56d0a8b4982346465d9
# Thu, 10 Nov 2022 00:38:27 GMT
ENV _BASH_VERSION=devel-20221107
# Thu, 10 Nov 2022 00:39:24 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Thu, 10 Nov 2022 00:39:26 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 10 Nov 2022 00:39:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 00:39:27 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:6c0d3b419d848ea31ca748254611d5d5ce3b76e3d7bba520fd87400fbb75f3b9`  
		Last Modified: Tue, 09 Aug 2022 17:39:33 GMT  
		Size: 2.8 MB (2807121 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a2789040161c40483a43fe9601c6dd674e80ff6ddb01dd37802cbb99ff63f1ec`  
		Last Modified: Thu, 10 Nov 2022 00:59:51 GMT  
		Size: 3.1 MB (3130966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af22a6731859c3f9973f2d846259641b7b85dcb3eb9b54ec5fa5cc9031632987`  
		Last Modified: Thu, 10 Nov 2022 00:59:50 GMT  
		Size: 341.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel` - linux; ppc64le

```console
$ docker pull bash@sha256:bba004ec7c8548ccdabef40ffa1c46024840e14dc4d67eb626628e808b959cbf
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 MB (6246151 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1db1b2324926ec3af29398c63db9f3945f4b8dcdf19b499859d23f9e017f6d2e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Aug 2022 17:17:09 GMT
ADD file:66b351666e41834033d334aeb3dc6998dea77aa22e8e254028c923fee67a41a8 in / 
# Tue, 09 Aug 2022 17:17:10 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 01:16:29 GMT
ENV _BASH_COMMIT=31f4d468b60eb27d768ef56d0a8b4982346465d9
# Thu, 10 Nov 2022 01:16:29 GMT
ENV _BASH_VERSION=devel-20221107
# Thu, 10 Nov 2022 01:17:44 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Thu, 10 Nov 2022 01:17:44 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 10 Nov 2022 01:17:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 01:17:46 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:c79e5d1a8c89b87020a754c8a5c8370faaa37bfb5bca1d8af66770d522ef1caf`  
		Last Modified: Tue, 09 Aug 2022 17:18:26 GMT  
		Size: 2.8 MB (2803320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a40bb9c001079fe78719a4d51e6e5d4f339701930932dc16045440a3a1f5a8c`  
		Last Modified: Thu, 10 Nov 2022 01:38:53 GMT  
		Size: 3.4 MB (3442487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:98d22b832145ec3cf8a2665ed7210d1176b984051c0e922f0d6294fa8b506ae8`  
		Last Modified: Thu, 10 Nov 2022 01:38:51 GMT  
		Size: 344.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `bash:devel` - linux; s390x

```console
$ docker pull bash@sha256:2ac2d04c6ee4cedfb79dc5fba823c4aae309b3cdea6b9f9dee5c4e5be5511e1d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.8 MB (5772369 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:866a4cc9eefbab599a942b021d375b6937545b4940a6d1d591151796f3815142`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["bash"]`

```dockerfile
# Tue, 09 Aug 2022 17:41:46 GMT
ADD file:b43a065471bc4711415d3c67cd5b6559b0c48ee7ffe9761530477cf457a6dc34 in / 
# Tue, 09 Aug 2022 17:41:46 GMT
CMD ["/bin/sh"]
# Thu, 10 Nov 2022 00:41:35 GMT
ENV _BASH_COMMIT=31f4d468b60eb27d768ef56d0a8b4982346465d9
# Thu, 10 Nov 2022 00:41:35 GMT
ENV _BASH_VERSION=devel-20221107
# Thu, 10 Nov 2022 00:42:21 GMT
RUN set -eux; 		apk add --no-cache --virtual .build-deps 		bison 		coreutils 		dpkg-dev dpkg 		gcc 		libc-dev 		make 		ncurses-dev 		tar 	; 		wget -O bash.tar.gz "https://git.savannah.gnu.org/cgit/bash.git/snapshot/bash-$_BASH_COMMIT.tar.gz"; 		mkdir -p /usr/src/bash; 	tar 		--extract 		--file=bash.tar.gz 		--strip-components=1 		--directory=/usr/src/bash 	; 	rm bash.tar.gz; 		if [ -d bash-patches ]; then 		apk add --no-cache --virtual .patch-deps patch; 		for p in bash-patches/*; do 			patch 				--directory=/usr/src/bash 				--input="$(readlink -f "$p")" 				--strip=0 			; 			rm "$p"; 		done; 		rmdir bash-patches; 		apk del --no-network .patch-deps; 	fi; 		cd /usr/src/bash; 	gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-readline 		--with-curses 		--without-bash-malloc 	|| { 		cat >&2 config.log; 		false; 	}; 	make -j "$(nproc)"; 	make install; 	cd /; 	rm -r /usr/src/bash; 		rm -rf 		/usr/local/share/doc/bash/*.html 		/usr/local/share/info 		/usr/local/share/locale 		/usr/local/share/man 	; 		runDeps="$( 		scanelf --needed --nobanner --format '%n#p' --recursive /usr/local 			| tr ',' '\n' 			| sort -u 			| awk 'system("[ -e /usr/local/lib/" $1 " ]") == 0 { next } { print "so:" $1 }' 	)"; 	apk add --no-network --virtual .bash-rundeps $runDeps; 	apk del --no-network .build-deps; 		[ "$(which bash)" = '/usr/local/bin/bash' ]; 	bash --version; 	bash -c 'help' > /dev/null
# Thu, 10 Nov 2022 00:42:22 GMT
COPY file:651b3bebeba8be9162c56b3eb561199905235f3e1c7811232b6c9f48ac333651 in /usr/local/bin/ 
# Thu, 10 Nov 2022 00:42:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 10 Nov 2022 00:42:23 GMT
CMD ["bash"]
```

-	Layers:
	-	`sha256:790c84f1f3409eab952345157df7fa804ba6b5f06d4ceb6f2dfa3c6de2064397`  
		Last Modified: Tue, 09 Aug 2022 17:42:45 GMT  
		Size: 2.6 MB (2590597 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea8aa3406a146e46e68ee1e9f577292e02966031f77dcd3e8c87636adda2e8b`  
		Last Modified: Thu, 10 Nov 2022 00:58:49 GMT  
		Size: 3.2 MB (3181432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cdcaedcc3cab6ac89dcb3a7827e690e3f06a97f6b4d7eedefa9026a45294c0b`  
		Last Modified: Thu, 10 Nov 2022 00:58:48 GMT  
		Size: 340.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
