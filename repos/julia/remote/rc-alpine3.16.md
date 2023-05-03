## `julia:rc-alpine3.16`

```console
$ docker pull julia@sha256:ae81e6dc2d59b4cda43271658cac40b897c409ae59728a1840b8974b66a2e7c8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `julia:rc-alpine3.16` - linux; amd64

```console
$ docker pull julia@sha256:3385522bde4eae985808df43df15bd3758a788820c62692ec22e722545bdc03d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **153.4 MB (153414906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7d433347bd385902111da4e072f0ffeb212982d81c55d54dcac33cc125adbf26`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:28 GMT
ADD file:970e6b2578ef73457ffed1189e8ba128b0211cabd3174b8c7d3afd8fb58ad614 in / 
# Wed, 29 Mar 2023 18:19:28 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 22:05:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 29 Mar 2023 22:05:09 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 22:05:09 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 03 May 2023 04:16:05 GMT
ENV JULIA_VERSION=1.9.0-rc3
# Wed, 03 May 2023 04:16:18 GMT
RUN set -eux; 		apk add --no-cache --virtual .fetch-deps gnupg; 		arch="$(apk --print-arch)"; 	case "$arch" in 		'x86_64') 			url='https://julialang-s3.julialang.org/bin/musl/x64/1.9/julia-1.9.0-rc3-musl-x86_64.tar.gz'; 			sha256='bce9620d7fb1b3fe851aebc71ab24323ceb321e6f73789f672244fef73209662'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		wget -O julia.tar.gz.asc "$url.asc"; 	wget -O julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum -w -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apk del --no-network .fetch-deps; 		julia --version
# Wed, 03 May 2023 04:16:19 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 03 May 2023 04:16:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 03 May 2023 04:16:20 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:91d30c5bc19582de1415b18f1ec5bcbf52a558b62cf6cc201c9669df9f748c22`  
		Last Modified: Wed, 29 Mar 2023 18:20:09 GMT  
		Size: 2.8 MB (2807803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f29b23b9d159fdd7adb35517d4cb5e2ed111f5e7705e8e0d2007aaebd3f5cb48`  
		Last Modified: Wed, 03 May 2023 04:21:13 GMT  
		Size: 150.6 MB (150606729 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d468b72fb0f1e49cf5612f8fbf405d9cfe044118daec4595c89c6a7d41df8298`  
		Last Modified: Wed, 03 May 2023 04:20:50 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
