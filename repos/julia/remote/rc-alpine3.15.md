## `julia:rc-alpine3.15`

```console
$ docker pull julia@sha256:694be69d6412ae67d3bb19e4912bba692484e03b3980b91af57640a7bdc79c1c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:rc-alpine3.15` - linux; amd64

```console
$ docker pull julia@sha256:0574045968a8bd23d7b0605576bcd1f3a4a4ae28bd2a40bf4ddc03aa38d66e33
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.2 MB (151238084 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:25709f5a24e191ed1de577651317535745442292c03decec59ab8b32ee44967b`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 05 Apr 2022 00:19:59 GMT
ADD file:5d673d25da3a14ce1f6cf66e4c7fd4f4b85a3759a9d93efb3fd9ff852b5b56e4 in / 
# Tue, 05 Apr 2022 00:19:59 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:10:17 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 05 Apr 2022 07:10:17 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 07:10:17 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 02 Jun 2022 18:34:21 GMT
ENV JULIA_VERSION=1.8.0-rc1
# Thu, 02 Jun 2022 18:34:37 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.8/julia-1.8.0-rc1-musl-x86_64.tar.gz'; 			sha256='fb78d1547fd3a82881ccc8d3d5bb24310c59feb08473e0a05d5d44314f23b195'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 02 Jun 2022 18:34:39 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ecc826158bb1031e28f70b1011f255cef9fe7cf0d890ce36490d531261fdb2d`  
		Last Modified: Thu, 02 Jun 2022 18:38:06 GMT  
		Size: 148.4 MB (148423525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
