## `julia:1-alpine`

```console
$ docker pull julia@sha256:9e6ef51c49e94b105223711c09f121d84b7e47650abd7d8aeafc847824efc3eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine` - linux; amd64

```console
$ docker pull julia@sha256:10bf0f8a859d70322ecb4c40d0e50b1198ac442dff02d4d64ff601f33d246772
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154540826 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6806a2bbfee12317abafc8e4fa0a982f67ba37bbea3f060a3c50a870dd7ae496`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:41:58 GMT
ADD file:1da756d12551a0e3e793e02ef87432d69d4968937bd11bed0af215db19dd94cd in / 
# Wed, 14 Jun 2023 20:41:59 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:24:41 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:24:54 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.2-musl-x86_64.tar.gz'; 			sha256='8fb6c39d44eeed91acade4b649777871a7a8485ae7e0aaaf47e59103d13bce31'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 06 Jul 2023 20:24:56 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:24:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:24:56 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:31e352740f534f9ad170f75378a84fe453d6156e40700b882d737a8f4a6988a3`  
		Last Modified: Wed, 14 Jun 2023 20:42:26 GMT  
		Size: 3.4 MB (3397879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176aed722f5b78566ab7201194bd215b19fa171f06d776d6af17ccd1088f8e32`  
		Last Modified: Thu, 06 Jul 2023 20:27:32 GMT  
		Size: 151.1 MB (151142577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:349a1e3ff684d5591503f149f6afbe19321d2cc048890e59e216ff84c74eae53`  
		Last Modified: Thu, 06 Jul 2023 20:27:10 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
