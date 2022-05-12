## `julia:rc-alpine3.15`

```console
$ docker pull julia@sha256:d5c1e6357ae594fb71a459e2cf523fa1806e909ea6b4c153e17d45912b23d5d3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:rc-alpine3.15` - linux; amd64

```console
$ docker pull julia@sha256:9f5a6c5a6d57992e825b7edb502e326ff7f68efadae0305d1e5643133872862b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.6 MB (145572535 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b77d3773760714d42c3abd000c83f802d7ac7c922aae357493353e64dd74d10`
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
# Tue, 05 Apr 2022 07:10:17 GMT
ENV JULIA_VERSION=1.8.0-beta3
# Tue, 05 Apr 2022 07:10:35 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.8/julia-1.8.0-beta3-musl-x86_64.tar.gz'; 			sha256='88fcc6b603e642d4884ba63c653a4885e74a715a982d0fda30e07f9f65e13540'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 05 Apr 2022 07:10:36 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:df9b9388f04ad6279a7410b85cedfdcb2208c0a003da7ab5613af71079148139`  
		Last Modified: Mon, 04 Apr 2022 19:10:16 GMT  
		Size: 2.8 MB (2814559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c989f4e45d68f749879d80aaf33b425086d6f40c4e2ece5866a54d4a490d05f`  
		Last Modified: Tue, 05 Apr 2022 07:13:24 GMT  
		Size: 142.8 MB (142757976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
