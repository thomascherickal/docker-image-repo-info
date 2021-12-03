## `julia:1-alpine3.15`

```console
$ docker pull julia@sha256:54a1025f61898e4dd009645fe991e5595c1df92dd03f2ee3b2c654534ba8e6ac
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:1-alpine3.15` - linux; amd64

```console
$ docker pull julia@sha256:7e5893f4c4f1bd19719f1105e121bd656fe217629fd76bffeac6b0c60ce4e661
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **134.4 MB (134442860 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9f6f4f2a7beb22952619669919fab7e89235a174b7841ea3e39ecf4e65891f4b`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 24 Nov 2021 20:19:40 GMT
ADD file:9233f6f2237d79659a9521f7e390df217cec49f1a8aa3a12147bbca1956acdb9 in / 
# Wed, 24 Nov 2021 20:19:40 GMT
CMD ["/bin/sh"]
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 01 Dec 2021 02:25:12 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 01 Dec 2021 02:25:12 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Fri, 03 Dec 2021 20:32:55 GMT
ENV JULIA_VERSION=1.7.0
# Fri, 03 Dec 2021 20:33:12 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.7/julia-1.7.0-musl-x86_64.tar.gz'; 			sha256='c39d9937ebdb693ce69f8695ac55bdd1c8b8557fca38d72cd6e467e05258fc8f'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Fri, 03 Dec 2021 20:33:13 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:59bf1c3509f33515622619af21ed55bbe26d24913cedbca106468a5fb37a50c3`  
		Last Modified: Wed, 24 Nov 2021 20:20:05 GMT  
		Size: 2.8 MB (2818413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22abbb3b5471c36fa7d2ec98acd454bf76d20796f4576cc691f851fabdd6831c`  
		Last Modified: Fri, 03 Dec 2021 20:37:24 GMT  
		Size: 131.6 MB (131624447 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
