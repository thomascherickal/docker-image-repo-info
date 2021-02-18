## `julia:1-alpine3.13`

```console
$ docker pull julia@sha256:449399b62ad593b3a2f1dc513d577f84ab4802a19007e960cc60f73c8dac7c5c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `julia:1-alpine3.13` - linux; amd64

```console
$ docker pull julia@sha256:1e81f6059d8102d322c49f64a03edab5305312ba39edc77c4785d80dd5ec5972
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **112.5 MB (112522080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:52aae5675258a447f95c7fe8ef4e97ad15ef91eb566bf3fd3b0a233f94f8f897`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Wed, 17 Feb 2021 23:41:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 17 Feb 2021 23:41:44 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 17 Feb 2021 23:41:45 GMT
ENV JULIA_VERSION=1.5.3
# Wed, 17 Feb 2021 23:42:04 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		apkArch="$(apk --print-arch)"; 	case "$apkArch" in 		x86_64) tarArch='x86_64'; dirArch='x64'; sha256='2faf4ebe3b5fa1bbee853655ef7c292b457e80d3fca1af1c8d3f179286b27da6' ;; 		*) echo >&2 "error: current architecture ($apkArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	wget -O julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz.asc"; 	wget -O julia.tar.gz     "https://julialang-s3.julialang.org/bin/musl/${dirArch}/${folder}/julia-${JULIA_VERSION}-musl-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 17 Feb 2021 23:42:05 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3476147b582f3fe6a571b903053e607cc495a0537e9c2d71c43de91d942a8f7`  
		Last Modified: Wed, 17 Feb 2021 23:43:16 GMT  
		Size: 109.7 MB (109710423 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
