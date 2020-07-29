## `julia:rc-buster`

```console
$ docker pull julia@sha256:9490c6cd0b76fc06c66ace4fb2e7d9af764aa18ea2e243c10b0e118d67b94494
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:rc-buster` - linux; amd64

```console
$ docker pull julia@sha256:75e6657b0ef661830b47e98497e99f1bc61b647061a2aae44273b9ca4d1f8c1f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **144.4 MB (144402558 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ce07dfeb31912c8b5b2494769e4197ed8fccc1ace5654e665bea8f430fc33fb`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 22 Jul 2020 02:03:37 GMT
ADD file:6ccb3bbcc69b0d44c48a8ef1bfa08d835444ea13b8a93701bd37d86b81b13ac2 in / 
# Wed, 22 Jul 2020 02:03:37 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 20:09:06 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 20:09:06 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 22 Jul 2020 20:09:07 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Jul 2020 20:09:07 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 29 Jul 2020 01:19:42 GMT
ENV JULIA_VERSION=1.5.0-rc2
# Wed, 29 Jul 2020 01:20:00 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='b830c75e0839902337a59b0eb3db73b8d1d79c2a548b32b204c82486748bd78c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1034d1e5d4793fd46cd02f5df2eb3c5380d42d01146df3615f66d8848eb9ff3d' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='983161f0b96de0e1d6e5e7690f8b50d4ac20761a2472db228a03a484fe7c7086' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 29 Jul 2020 01:20:01 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:6ec8c9369e08152361a01729f2c8a1e7aae898426c6e67267f41894bf9524827`  
		Last Modified: Wed, 22 Jul 2020 02:09:51 GMT  
		Size: 27.1 MB (27098544 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f94669dc25b456ec3bf92cfb40d1a02e0c69cfe297caf9bf5113ccdc43016524`  
		Last Modified: Wed, 22 Jul 2020 20:11:40 GMT  
		Size: 4.4 MB (4436686 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cc90629a806b4cca9b32f9b0dfa03e4c9ba20ad0b1de066c91c65ef6c3ab7816`  
		Last Modified: Wed, 29 Jul 2020 01:21:09 GMT  
		Size: 112.9 MB (112867328 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:5bae9bb280a89bad29c509957af1d83c5d45d28dbb43cf30f2c53b94e1357b49
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.5 MB (135473664 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76620dacfb1b9435040ed09e016d631aff207d4c9c6d5d2953223b3619a728b8`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 22 Jul 2020 00:41:09 GMT
ADD file:1efd5b51a56f36bcf79a1bcea1df36ef28299a42bc11e758f9e49066f2a1f085 in / 
# Wed, 22 Jul 2020 00:41:10 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 05:19:37 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 05:19:38 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 22 Jul 2020 05:19:39 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Jul 2020 05:19:39 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 29 Jul 2020 00:40:11 GMT
ENV JULIA_VERSION=1.5.0-rc2
# Wed, 29 Jul 2020 00:40:51 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='b830c75e0839902337a59b0eb3db73b8d1d79c2a548b32b204c82486748bd78c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1034d1e5d4793fd46cd02f5df2eb3c5380d42d01146df3615f66d8848eb9ff3d' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='983161f0b96de0e1d6e5e7690f8b50d4ac20761a2472db228a03a484fe7c7086' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 29 Jul 2020 00:40:54 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3999339def4d7591a8064bfc698302ae0e29bc5e0557ae392c122e1b3efa9305`  
		Last Modified: Wed, 22 Jul 2020 00:47:42 GMT  
		Size: 25.9 MB (25857826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df97cd25183cc6965c04b8c10518194e9816680eef473a12d4f5abaa187fc993`  
		Last Modified: Wed, 22 Jul 2020 05:23:21 GMT  
		Size: 4.3 MB (4315195 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e3abfbd33db0ea719016e58ae566c93342f4e837c7ecf606a7d394c0d0e7fc5c`  
		Last Modified: Wed, 29 Jul 2020 00:42:09 GMT  
		Size: 105.3 MB (105300643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-buster` - linux; 386

```console
$ docker pull julia@sha256:fb04d61bd88a3b518926541a7915a29f9140266315db990d466c3e10b7a93a86
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **142.2 MB (142242277 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2462a1da70e3a5b7673905e172aa5d47aecffe6b95c1dca84091412d93e7b6a4`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 22 Jul 2020 02:09:15 GMT
ADD file:ee51bd8fcf2e02243de32c0f0e7899acebfa23bdceb783f13feb33c484ee98b8 in / 
# Wed, 22 Jul 2020 02:09:15 GMT
CMD ["bash"]
# Wed, 22 Jul 2020 08:07:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 22 Jul 2020 08:07:50 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 22 Jul 2020 08:07:50 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 22 Jul 2020 08:07:51 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 29 Jul 2020 00:38:35 GMT
ENV JULIA_VERSION=1.5.0-rc2
# Wed, 29 Jul 2020 00:38:58 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='b830c75e0839902337a59b0eb3db73b8d1d79c2a548b32b204c82486748bd78c' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='1034d1e5d4793fd46cd02f5df2eb3c5380d42d01146df3615f66d8848eb9ff3d' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='983161f0b96de0e1d6e5e7690f8b50d4ac20761a2472db228a03a484fe7c7086' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 29 Jul 2020 00:38:58 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:75157e9ef5a857d6b02d235e08a164737ad009bae299277f86131063e6204e0b`  
		Last Modified: Wed, 22 Jul 2020 02:15:45 GMT  
		Size: 27.8 MB (27754899 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cbacfbbc9ba8628851d4fae2e19c0c889802c10422021fbf83510e7b5379c5d`  
		Last Modified: Wed, 22 Jul 2020 08:11:05 GMT  
		Size: 4.6 MB (4585889 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaf312536dc1513e021fbbb5d08a6401c1f9c88175f9f04e9d9342f8e19cd14`  
		Last Modified: Wed, 29 Jul 2020 00:39:55 GMT  
		Size: 109.9 MB (109901489 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
