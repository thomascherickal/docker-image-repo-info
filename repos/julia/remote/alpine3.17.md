## `julia:alpine3.17`

```console
$ docker pull julia@sha256:d5c4035b68e660e213772c08e46a9efb70895aa397f664dda89344cf1b066bd7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:alpine3.17` - linux; amd64

```console
$ docker pull julia@sha256:2e3b7d449f63f6759404bf3e414164559d8b56d076ae10a7d9493b153dccefca
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **154.5 MB (154517691 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5fecf32bc21e8f19277b73f5ae1fbfbb7f61996eec72e6db0b3c341c0d83c35f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 14 Jun 2023 20:42:04 GMT
ADD file:828b07e74c184e7f251ed992ff195cdc50fdca345f13ff484e258851d928d950 in / 
# Wed, 14 Jun 2023 20:42:04 GMT
CMD ["/bin/sh"]
# Thu, 15 Jun 2023 00:14:34 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 15 Jun 2023 00:14:34 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 15 Jun 2023 00:14:34 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 06 Jul 2023 20:25:01 GMT
ENV JULIA_VERSION=1.9.2
# Thu, 06 Jul 2023 20:25:15 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.2-musl-x86_64.tar.gz'; 			sha256='8fb6c39d44eeed91acade4b649777871a7a8485ae7e0aaaf47e59103d13bce31'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Thu, 06 Jul 2023 20:25:17 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Thu, 06 Jul 2023 20:25:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 06 Jul 2023 20:25:17 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:4db1b89c0bd13344176ddce2d093b9da2ae58336823ffed2009a7ea4b62d2a95`  
		Last Modified: Wed, 14 Jun 2023 20:42:37 GMT  
		Size: 3.4 MB (3374713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09aca3cbabb864e81b14b1cf75dee6cb4a5c034a5c4d529b4dd548c708ad7585`  
		Last Modified: Thu, 06 Jul 2023 20:28:15 GMT  
		Size: 151.1 MB (151142605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5584a8659f45d6418de9bea871a53ad36743c215f9cdcc65b2bf41c93df8f8eb`  
		Last Modified: Thu, 06 Jul 2023 20:27:53 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
