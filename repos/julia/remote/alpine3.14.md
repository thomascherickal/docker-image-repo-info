## `julia:alpine3.14`

```console
$ docker pull julia@sha256:8d694f350ed9d13a457d7d33a951594ef7b55cd8a60b5dac116366ffe2fc6920
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine3.14` - linux; amd64

```console
$ docker pull julia@sha256:4328442d3c3eb9de31aec772546436b7a9b38ba319a274ad8282e7388c7747c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134595199 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4b5683a72eb9212724b391b9bbe160fecbec5b864b8f7b4432d2d5cf73e75359`
-	Default Command: `["julia"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 06:02:16 GMT
ENV JULIA_PATH=/usr/local/julia
# Sat, 13 Nov 2021 06:02:16 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Sat, 13 Nov 2021 06:02:17 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 27 Dec 2021 18:45:31 GMT
ENV JULIA_VERSION=1.7.1
# Mon, 27 Dec 2021 18:45:52 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.7/julia-1.7.1-musl-x86_64.tar.gz'; 			sha256='cf94c4686dfcc4a22e6d0ec42a5f752c1c4ac55a32014851b030e62c20519fad'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Mon, 27 Dec 2021 18:45:53 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1053bc232f4e5495d158a20c62c5fca1d2b6f2741a93580531bf266910062a8f`  
		Last Modified: Mon, 27 Dec 2021 18:48:49 GMT  
		Size: 131.8 MB (131772218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
