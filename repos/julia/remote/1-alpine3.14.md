## `julia:1-alpine3.14`

```console
$ docker pull julia@sha256:1d69a694ae49757b9d80d88d92e73faded3b65da6a86185e95706db9c674d500
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine3.14` - linux; amd64

```console
$ docker pull julia@sha256:9e65da7bf624d64b7ca84fb8514211de95dbd9f9d020af5c1a4cd72286d3d9da
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134447391 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:39873c4f2cbaf7fd856eb5ef2b6a5a914a798dc478bc7861c3420bd08a0993ea`
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
# Fri, 03 Dec 2021 20:33:17 GMT
ENV JULIA_VERSION=1.7.0
# Fri, 03 Dec 2021 20:33:30 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.7/julia-1.7.0-musl-x86_64.tar.gz'; 			sha256='c39d9937ebdb693ce69f8695ac55bdd1c8b8557fca38d72cd6e467e05258fc8f'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 03 Dec 2021 20:33:31 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e53ad73cc4700ffa66062f3efee379c785bb926633a78649e349a93b0b2fc29d`  
		Last Modified: Fri, 03 Dec 2021 20:38:08 GMT  
		Size: 131.6 MB (131624410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
