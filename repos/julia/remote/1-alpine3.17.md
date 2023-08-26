## `julia:1-alpine3.17`

```console
$ docker pull julia@sha256:65bfe903d60f9fde0be7b02d5647bc313383a9f0e451c66bf99d6c9af2098e8a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine3.17` - linux; amd64

```console
$ docker pull julia@sha256:405760203b2ff5d3bf2f90cadc18db9a639d2757ecc7c3d38f2366f9dc6e8345
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.4 MB (154359946 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe88216bd7a333dd18524056e1e5e2575e571ff31480e4e3d81d2a7d19d12d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Mon, 07 Aug 2023 19:20:26 GMT
ADD file:6dd87346b8be240b21b4f4d9296253bf0d28b6579aa52d2118872e3936963b6b in / 
# Mon, 07 Aug 2023 19:20:26 GMT
CMD ["/bin/sh"]
# Wed, 09 Aug 2023 02:00:23 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 09 Aug 2023 02:00:23 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 09 Aug 2023 02:00:23 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Sat, 26 Aug 2023 04:06:03 GMT
ENV JULIA_VERSION=1.9.3
# Sat, 26 Aug 2023 04:06:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.3-musl-x86_64.tar.gz'; 			sha256='90fbfb8621a523694de0280a1cd5e2040a49f4bd41e403f789caee945e63d03b'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Sat, 26 Aug 2023 04:06:19 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Sat, 26 Aug 2023 04:06:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 26 Aug 2023 04:06:19 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9398808236ffac29e60c04ec906d8d409af7fa19dc57d8c65ad167e9c4967006`  
		Last Modified: Mon, 07 Aug 2023 19:21:08 GMT  
		Size: 3.4 MB (3378609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c12b6570d0e9bc63eeb51f87fafd7654563ed50fd2405a27a3d0015afc9b37c6`  
		Last Modified: Sat, 26 Aug 2023 04:11:50 GMT  
		Size: 151.0 MB (150980967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93c839ba6bad9d8366856149b1ab28b0d212b989b57734a12af4830eb9d9febe`  
		Last Modified: Sat, 26 Aug 2023 04:11:27 GMT  
		Size: 370.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
