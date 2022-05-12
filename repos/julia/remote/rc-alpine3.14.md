## `julia:rc-alpine3.14`

```console
$ docker pull julia@sha256:8a3c8f29cd07c96dbc80b6b610f9252c1c02f505749a8236326a82d07c8b6679
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:rc-alpine3.14` - linux; amd64

```console
$ docker pull julia@sha256:7a70fabd82b9440d1a211106795cf3520472bc691a0860c36eddb8e3bdd0b908
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **145.6 MB (145576031 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e613fb24225109ad84ad616d1ec9831864ea70925417b24c8d9633b1a34c0de5`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Tue, 05 Apr 2022 07:10:40 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 05 Apr 2022 07:10:40 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 05 Apr 2022 07:10:40 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 05 Apr 2022 07:10:40 GMT
ENV JULIA_VERSION=1.8.0-beta3
# Tue, 05 Apr 2022 07:10:53 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.8/julia-1.8.0-beta3-musl-x86_64.tar.gz'; 			sha256='88fcc6b603e642d4884ba63c653a4885e74a715a982d0fda30e07f9f65e13540'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 05 Apr 2022 07:10:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1f40ba5057d33006d35c87e8bb03172419af0294c9c40f8d4034d05dbc14fd0`  
		Last Modified: Tue, 05 Apr 2022 07:14:00 GMT  
		Size: 142.8 MB (142757661 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
