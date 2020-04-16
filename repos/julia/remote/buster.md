## `julia:buster`

```console
$ docker pull julia@sha256:95190942275e9d93d98b3cea207f1712f454ad605e2a5dc39d33d8705c4c2cdc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386

### `julia:buster` - linux; amd64

```console
$ docker pull julia@sha256:f6697fd2dadbe5cd99a8b7f439b55b5767a62e36033a0b126f18696fa572ee36
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **138.3 MB (138329570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b01eb4abbeec2377ecff60cba5d329ba45487418f4e003df845bc0340e2898e3`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 03:22:36 GMT
ADD file:865f9041e12eb341f0a394764ddc11db49cbc8b91d4fb57c6fb1960b68b1bb41 in / 
# Thu, 16 Apr 2020 03:22:36 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 08:58:09 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 08:58:09 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 08:58:10 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 08:58:10 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 08:58:10 GMT
ENV JULIA_VERSION=1.4.0
# Thu, 16 Apr 2020 08:58:34 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 08:58:34 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:123275d6e508d282237a22fefa5aef822b719a06496444ea89efa65da523fc4b`  
		Last Modified: Thu, 16 Apr 2020 03:31:44 GMT  
		Size: 27.1 MB (27098147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1003677cbe41c0cefc546b2e7b389164738d011ef1223d66fd1b78f55a36cf8e`  
		Last Modified: Thu, 16 Apr 2020 09:00:12 GMT  
		Size: 4.4 MB (4436586 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e73003eef18fb06dfbfd6c2c8709e76df09737983512eebacc0142e6b01e4862`  
		Last Modified: Thu, 16 Apr 2020 09:00:36 GMT  
		Size: 106.8 MB (106794837 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm variant v7

```console
$ docker pull julia@sha256:0ac7eb3ba05168cd26791bb2e36436f2fa132b37f0776a9b39fb36214bb93f47
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **123.5 MB (123503508 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:07f5de0dda095868608104228885ffc09b658a247d7720b16fc63282f0f26238`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 00:59:45 GMT
ADD file:e346a36a456d66d8019344b5f7d60df8b5b24aea1461c19838982135ad1f4d7d in / 
# Thu, 16 Apr 2020 00:59:47 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 04:25:42 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 04:25:44 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 04:25:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 04:25:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 04:25:49 GMT
ENV JULIA_VERSION=1.4.0
# Thu, 16 Apr 2020 04:26:28 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 04:26:30 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:838dc71644c10eab485c4bdfa3879e0fb9e72426de1239cfac1d4c05c23db7be`  
		Last Modified: Thu, 16 Apr 2020 01:08:59 GMT  
		Size: 22.7 MB (22705228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8af8b948b8398fdaedb31139f89a90df29ad9f05038a6de0ff9817c777763f`  
		Last Modified: Thu, 16 Apr 2020 04:28:43 GMT  
		Size: 3.8 MB (3783579 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0230b466eb1f16bd472b786b23f9da3b9174ac5b23eab9e862321830d0c2d0e`  
		Last Modified: Thu, 16 Apr 2020 04:29:15 GMT  
		Size: 97.0 MB (97014701 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:32b9df939bda95bc97941d58de3cdffb6c0a8c5583bafad563fefc56ca06c77f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **119.9 MB (119881528 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5d61da508a4e1e1d16d25377a17742138cf2a1fe48b443d2c52266df6a26abd9`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 02:41:52 GMT
ADD file:1aab17002a9095c31dd6928277a045cb26846ac58c3d2d63316332c99a5f90bd in / 
# Thu, 16 Apr 2020 02:41:57 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:31:45 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 06:31:46 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 06:31:47 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 06:31:48 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 06:31:48 GMT
ENV JULIA_VERSION=1.4.0
# Thu, 16 Apr 2020 06:32:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 06:32:18 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:3d48095d71a365b5910cea98e5566c152a3f9aa11657560568259bf93ff2f4cb`  
		Last Modified: Thu, 16 Apr 2020 02:48:58 GMT  
		Size: 25.9 MB (25857715 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:529c1540c7ec92a7145151f1ecc07feff4c396e844d01531c3ad248a2cdfd537`  
		Last Modified: Thu, 16 Apr 2020 06:34:22 GMT  
		Size: 4.3 MB (4315529 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c01a8d763903e1012c1728eb25b43b8c33819f50d9fb18c7b6e30c100c86f5bb`  
		Last Modified: Thu, 16 Apr 2020 06:34:48 GMT  
		Size: 89.7 MB (89708284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:buster` - linux; 386

```console
$ docker pull julia@sha256:6387d1da06ebe86ba8656a74aea893da34e8965ace0fe71a0e8cfa9d35047d98
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **135.8 MB (135752129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6eb4cb985ba83b2125420e6d40f4251910be1036cc39b7c5f248b1694f167fe0`
-	Default Command: `["julia"]`

```dockerfile
# Thu, 16 Apr 2020 01:39:55 GMT
ADD file:ab0bbfba6c4b56420ffffc6cdddcc4592fff018f0cd07578c7dc0a5faa49df2f in / 
# Thu, 16 Apr 2020 01:39:56 GMT
CMD ["bash"]
# Thu, 16 Apr 2020 06:03:10 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 16 Apr 2020 06:03:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Thu, 16 Apr 2020 06:03:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 16 Apr 2020 06:03:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Thu, 16 Apr 2020 06:03:12 GMT
ENV JULIA_VERSION=1.4.0
# Thu, 16 Apr 2020 06:03:41 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi; 		dpkgArch="$(dpkg --print-architecture)"; 	case "${dpkgArch##*-}" in 		amd64) tarArch='x86_64'; dirArch='x64'; sha256='30d126dc3598f3cd0942de21cc38493658037ccc40eb0882b3b4c418770ca751' ;; 		armhf) tarArch='armv7l'; dirArch='armv7l'; sha256='6f7f9407485c8f1380e34a751305eb70a1da9d05af8f882ffaed4e1a09effd56' ;; 		arm64) tarArch='aarch64'; dirArch='aarch64'; sha256='576481accadd441655edf963b81c28cbeaa327b423ec58a77eab103cf830a65a' ;; 		i386) tarArch='i686'; dirArch='x86'; sha256='41ed8cce4cb8a66dd84095f713bc50d85342e6794fb5f35ac6dafba3276d119d' ;; 		*) echo >&2 "error: current architecture ($dpkgArch) does not have a corresponding Julia binary release"; exit 1 ;; 	esac; 		folder="$(echo "$JULIA_VERSION" | cut -d. -f1-2)"; 	curl -fL -o julia.tar.gz.asc "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz.asc"; 	curl -fL -o julia.tar.gz     "https://julialang-s3.julialang.org/bin/linux/${dirArch}/${folder}/julia-${JULIA_VERSION}-linux-${tarArch}.tar.gz"; 		echo "${sha256} *julia.tar.gz" | sha256sum -c -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver ha.pool.sks-keyservers.net --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	command -v gpgconf > /dev/null && gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Thu, 16 Apr 2020 06:03:41 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:75bc60a98e6523be3fadd9128c1a630cb5cbd2d2d813ee5e99dc146a3de22254`  
		Last Modified: Thu, 16 Apr 2020 01:46:20 GMT  
		Size: 27.8 MB (27753976 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e047836a1122c19b6c47bef4f71c487c4036f81577e1bf9f4895e0c583b35cb`  
		Last Modified: Thu, 16 Apr 2020 06:05:30 GMT  
		Size: 4.6 MB (4586432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c11e62cb57a87b5ce7d8b77a900bbf995db1f133d0353b236e1d131f6631a44`  
		Last Modified: Thu, 16 Apr 2020 06:06:09 GMT  
		Size: 103.4 MB (103411721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
