## `julia:rc-alpine3.12`

```console
$ docker pull julia@sha256:c0c8976a24c4e4de3d766932c6e4a580f230bbb9b2d8f023b1ace6e933a821d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:rc-alpine3.12` - linux; amd64

```console
$ docker pull julia@sha256:b36126491e5c90f7783138c82de11c37c096639fdb889d22a428bae347caa312
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.4 MB (112423924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a730e6aca7c00eb00d7d19583449f59356b838154398a76b0347c268908e0537`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 29 May 2020 21:19:46 GMT
ADD file:c92c248239f8c7b9b3c067650954815f391b7bcb09023f984972c082ace2a8d0 in / 
# Fri, 29 May 2020 21:19:46 GMT
CMD ["/bin/sh"]
# Tue, 30 Jun 2020 22:19:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 30 Jun 2020 22:19:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 30 Jun 2020 22:19:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 30 Jun 2020 22:19:58 GMT
ENV JULIA_VERSION=1.5.0-rc1
# Tue, 30 Jun 2020 22:20:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='43e3a30133aee14657cc8984cc51e8f308ac1978e4c5986f4c976b8e8747194f' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 30 Jun 2020 22:20:18 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:df20fa9351a15782c64e6dddb2d4a6f50bf6d3688060a34c4014b0d9a752eb4c`  
		Last Modified: Fri, 29 May 2020 21:20:06 GMT  
		Size: 2.8 MB (2797541 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ec200ff2b9e1b58eae932cff65bea4c9366a288d0ba9efacd1aa1c73b4524f4`  
		Last Modified: Tue, 30 Jun 2020 22:21:21 GMT  
		Size: 109.6 MB (109626383 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
