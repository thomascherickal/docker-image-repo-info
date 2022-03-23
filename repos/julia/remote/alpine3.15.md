## `julia:alpine3.15`

```console
$ docker pull julia@sha256:9aea23e2a362308017eb6863e1faa5bce15f5ac924c72d306548c3c828413915
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine3.15` - linux; amd64

```console
$ docker pull julia@sha256:757e7eaf2d798e5de46a3173572ef2c86221f81bc42543d2105042711769c117
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.6 MB (134579924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a19f37e23fe616efca43527c57bff67833df4cde1bb8993da4c5a75aece0b3e5`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 23 Mar 2022 15:21:21 GMT
ADD file:7386ad893672007cca2d73cec1862d582a69d581ca1d155d4599cb2aa54d5498 in / 
# Wed, 23 Mar 2022 15:21:21 GMT
CMD ["/bin/sh"]
# Wed, 23 Mar 2022 18:06:04 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 23 Mar 2022 18:06:05 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 23 Mar 2022 18:06:05 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 23 Mar 2022 18:06:35 GMT
ENV JULIA_VERSION=1.7.2
# Wed, 23 Mar 2022 18:06:51 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.7/julia-1.7.2-musl-x86_64.tar.gz'; 			sha256='3bd653265f387450c796157629e6aa7aa4473d0169ef516a18e7b06b0301a7e1'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 23 Mar 2022 18:06:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3aa4d0bbde192bfaba75f2d124d8cf2e6de452ae03e55d54105e46b06eb8127e`  
		Last Modified: Wed, 23 Mar 2022 15:21:44 GMT  
		Size: 2.8 MB (2812689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:930e84fc187579648b580ea2d17e00930bcf297d18b11bf794c07decb360f6fc`  
		Last Modified: Wed, 23 Mar 2022 18:09:03 GMT  
		Size: 131.8 MB (131767235 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
