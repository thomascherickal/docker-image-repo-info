## `julia:rc-buster`

```console
$ docker pull julia@sha256:08c0f18c60565ab484d9af84a5fa066cb9a76202babfd9715c4c8768a704b3eb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:rc-buster` - linux; amd64

```console
$ docker pull julia@sha256:f5325efa87eaa85e4e6cbded515034e1f8275d7957857ef30ef1162b2f4ae339
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.2 MB (175221549 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3e43dc3961f478a30695dc7a1126c6bf8243536ff11dd749c98cca0a566726ce`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 11 May 2022 01:20:37 GMT
ADD file:76b454ddb7dfe4d22afae844a7e67e7e5fb4570dae2e21bbd259a1f2e5839f33 in / 
# Wed, 11 May 2022 01:20:37 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:37:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:37:47 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 11 May 2022 04:37:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 04:37:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 11 May 2022 04:37:48 GMT
ENV JULIA_VERSION=1.8.0-beta3
# Wed, 11 May 2022 04:38:03 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-beta3-linux-x86_64.tar.gz'; 			sha256='749b2f3c6832a7b34404838e579de94c369173250c07071383cb499f14812655'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-beta3-linux-aarch64.tar.gz'; 			sha256='43d23f114a2a8217f30072bb98613ed45a9930106dbe741577963571f186afc7'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-beta3-linux-i686.tar.gz'; 			sha256='4f10e62f02d7969f971f0497ccdd57656615f20d3e5ca4f206d0caf8b64ce1ca'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 11 May 2022 04:38:04 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c32ce6654453d35d0b3dde45d195adeee586ffba0a683006ee06748c077c01fa`  
		Last Modified: Wed, 11 May 2022 01:25:58 GMT  
		Size: 27.1 MB (27140722 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f835ab6eeb8f37becd7cbe24d50c8189e7c433230a112166c07b02c7b311119`  
		Last Modified: Wed, 11 May 2022 04:40:54 GMT  
		Size: 4.5 MB (4468152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81100c6275717a02fdd31f916303e853021082e00ad5d4d310704052a079b23c`  
		Last Modified: Wed, 11 May 2022 04:41:15 GMT  
		Size: 143.6 MB (143612675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:dd17fd542222f1cb474f7f9700333d5c63d75cf83d1ea0ae25421bb42d765260
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **167.4 MB (167416244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:beff4e174c13263f8fd5c3f0d350471109388ecd8dd3a2e7c22a0345d9f784da`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 11 May 2022 00:47:26 GMT
ADD file:2536146c773d09db1a8fbbff00933acc459d8929feb3cff5b93ca4c23b577845 in / 
# Wed, 11 May 2022 00:47:26 GMT
CMD ["bash"]
# Wed, 11 May 2022 02:21:27 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 02:21:27 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 11 May 2022 02:21:28 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 02:21:29 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 11 May 2022 02:21:30 GMT
ENV JULIA_VERSION=1.8.0-beta3
# Wed, 11 May 2022 02:21:44 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-beta3-linux-x86_64.tar.gz'; 			sha256='749b2f3c6832a7b34404838e579de94c369173250c07071383cb499f14812655'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-beta3-linux-aarch64.tar.gz'; 			sha256='43d23f114a2a8217f30072bb98613ed45a9930106dbe741577963571f186afc7'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-beta3-linux-i686.tar.gz'; 			sha256='4f10e62f02d7969f971f0497ccdd57656615f20d3e5ca4f206d0caf8b64ce1ca'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 11 May 2022 02:21:45 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:383d573fdcf2c6da56fdb61e120549d7bc200471208ca4c7c6605c57a0a87ef6`  
		Last Modified: Wed, 11 May 2022 00:54:36 GMT  
		Size: 25.9 MB (25909014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:635cdefb224fcf7fdd00c3708588b4c343f4b3d7abd1d3464f522caea509f6a2`  
		Last Modified: Wed, 11 May 2022 02:24:33 GMT  
		Size: 4.3 MB (4346901 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:54f156387a2fcb958b58d346695b7b2082666102a1dbce3644f923bc5758329c`  
		Last Modified: Wed, 11 May 2022 02:24:53 GMT  
		Size: 137.2 MB (137160329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-buster` - linux; 386

```console
$ docker pull julia@sha256:da1b6426350bbfd02ab1051d8cf029e90e70823a85f84f76d1d47ea29a504bb1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **171.1 MB (171115897 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:be16bad6ce719ce6c8dbd82370460acff109dcf098230b48967d4fdf437996d2`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 11 May 2022 01:39:41 GMT
ADD file:fc7b00a8a5b0e703ac3ede5e2e51257f5ee709fcd35fee53e7b99d144cd873e4 in / 
# Wed, 11 May 2022 01:39:42 GMT
CMD ["bash"]
# Wed, 11 May 2022 04:26:20 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 11 May 2022 04:26:21 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 11 May 2022 04:26:22 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 11 May 2022 04:26:23 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 11 May 2022 04:26:24 GMT
ENV JULIA_VERSION=1.8.0-beta3
# Wed, 11 May 2022 04:26:43 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.8/julia-1.8.0-beta3-linux-x86_64.tar.gz'; 			sha256='749b2f3c6832a7b34404838e579de94c369173250c07071383cb499f14812655'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.8/julia-1.8.0-beta3-linux-aarch64.tar.gz'; 			sha256='43d23f114a2a8217f30072bb98613ed45a9930106dbe741577963571f186afc7'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.8/julia-1.8.0-beta3-linux-i686.tar.gz'; 			sha256='4f10e62f02d7969f971f0497ccdd57656615f20d3e5ca4f206d0caf8b64ce1ca'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 11 May 2022 04:26:44 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b1c376c64b69c16b8b035dfd04b99bb7769a5afdfb56a1241aa4ec8743e85aa7`  
		Last Modified: Wed, 11 May 2022 01:47:22 GMT  
		Size: 27.8 MB (27799149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44763361e94a796a1177e74a30cf54fcd263fe26bf67befbe53acefd445f7949`  
		Last Modified: Wed, 11 May 2022 04:29:53 GMT  
		Size: 4.6 MB (4615843 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a6bcf503871045485f7b1921aff141ca16009678fef59f4b0fb0be6ecf72d5f`  
		Last Modified: Wed, 11 May 2022 04:30:12 GMT  
		Size: 138.7 MB (138700905 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
