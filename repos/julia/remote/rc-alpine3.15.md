## `julia:rc-alpine3.15`

```console
$ docker pull julia@sha256:7192f4a0638624292410bd355fa4c68e0a122cc59eca3427dd08947ac25e43f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:rc-alpine3.15` - linux; amd64

```console
$ docker pull julia@sha256:232de142d483349b2084d1135ed85d58ffe09a9e40eb14c73e768bf223fb91ef
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **151.4 MB (151431003 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:61319c123a63920a9eaeb270077ec2b6a89b484788614be380193d59cb8d20a9`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 09 Aug 2022 17:20:00 GMT
ADD file:f77e3f51f020890d22997e6c2ca98968b75b8bc8c463341a2010ff0655d4c88f in / 
# Tue, 09 Aug 2022 17:20:01 GMT
CMD ["/bin/sh"]
# Tue, 09 Aug 2022 20:42:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 09 Aug 2022 20:42:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 09 Aug 2022 20:42:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 09 Aug 2022 20:42:57 GMT
ENV JULIA_VERSION=1.8.0-rc3
# Tue, 09 Aug 2022 20:43:11 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.8/julia-1.8.0-rc3-musl-x86_64.tar.gz'; 			sha256='815d9d85382360a4caa3dfe39d64539ec32bf935e10098a116de3377a3feb2a6'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Tue, 09 Aug 2022 20:43:12 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:9621f1afde84053b2f9b6ff34fc7f7460712247c01cbab483c5fa7132cf782ca`  
		Last Modified: Tue, 09 Aug 2022 17:20:52 GMT  
		Size: 2.8 MB (2823512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6a2e3e8400047eca6c861108ddeef0f1ca26cf9e14628887f8888cf5452ce2b0`  
		Last Modified: Tue, 09 Aug 2022 20:46:36 GMT  
		Size: 148.6 MB (148607491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
