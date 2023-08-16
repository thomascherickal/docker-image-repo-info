## `julia:rc-bullseye`

```console
$ docker pull julia@sha256:49a5358820c4af2368c053891aa09f4b3882f2e629c0c5827a88b010c8716383
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le

### `julia:rc-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:5a2afa879ce3a22d7bd72d4c6166dd4b99ec855acbfad8baae33b593f9904bdc
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **200.8 MB (200798578 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:34cc1690ae7f0c4b15b8fc43a969c3e58deebff493cf1abfe7e3e5909bb6b1b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 16 Aug 2023 01:00:09 GMT
ADD file:2d91c2e03d02bfa16fe4f766d851b351d93d33f84751ad96c985e64ea024ec28 in / 
# Wed, 16 Aug 2023 01:00:09 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 09:58:02 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 09:58:02 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 16 Aug 2023 09:58:02 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 09:58:02 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 16 Aug 2023 09:58:02 GMT
ENV JULIA_VERSION=1.10.0-beta1
# Wed, 16 Aug 2023 09:58:20 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta1-linux-x86_64.tar.gz'; 			sha256='cda38a2dd5b0ec605cc07ffa44efd3e9fe1072db26525953d1e24fb432e0bf4f'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta1-linux-aarch64.tar.gz'; 			sha256='e8377819ca383c7f4ee1841169625c578123244c592882d8706b5bf45f58ea37'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta1-linux-i686.tar.gz'; 			sha256='fa5b6adfced2186a968fe36146e6103c4c6cc9aa849dfd1878644894eb28f0a7'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta1-linux-ppc64le.tar.gz'; 			sha256='8aa200030b6578334dcfc6404dbde8c894178b44d5eb88ec2b9bc8af8c8ce6e9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 16 Aug 2023 09:58:22 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 16 Aug 2023 09:58:22 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 09:58:22 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:14726c8f78342865030f97a8d3492e2d1a68fbd22778f9a31dc6be4b4f12a9bc`  
		Last Modified: Wed, 16 Aug 2023 01:05:12 GMT  
		Size: 31.4 MB (31417678 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d61aded178ba476c5d182b60e52edae6616cbaf5e09980250e129db7d9c4adec`  
		Last Modified: Wed, 16 Aug 2023 10:01:15 GMT  
		Size: 2.4 MB (2426694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f98f7a7b402f366164941a8bd2f27f8ec2dde0f78cd5851f1ac6b7a40225273c`  
		Last Modified: Wed, 16 Aug 2023 10:01:38 GMT  
		Size: 167.0 MB (166953833 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:573fea971b28c2c66bb2d4044d33f3f23841d99840d247e839fad00915d30f4f`  
		Last Modified: Wed, 16 Aug 2023 10:01:14 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:9d0575e259aa5b6c1318c7951f025b77d1aa3a8d074a9f1d0aff3279150ce2ed
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **194.1 MB (194084133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6108437d08cff0d9f245d2ddd1a9bc471a6b7c43ae0f2158e3cad60e6abc98f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 15 Aug 2023 23:40:11 GMT
ADD file:ea912fd82699af55c10b8136b5dc4b5ce9d08b8a01f9c06f6783d94dc430335a in / 
# Tue, 15 Aug 2023 23:40:11 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 03:30:05 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:30:06 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 16 Aug 2023 03:30:06 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 03:30:06 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 16 Aug 2023 03:30:06 GMT
ENV JULIA_VERSION=1.10.0-beta1
# Wed, 16 Aug 2023 03:30:23 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta1-linux-x86_64.tar.gz'; 			sha256='cda38a2dd5b0ec605cc07ffa44efd3e9fe1072db26525953d1e24fb432e0bf4f'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta1-linux-aarch64.tar.gz'; 			sha256='e8377819ca383c7f4ee1841169625c578123244c592882d8706b5bf45f58ea37'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta1-linux-i686.tar.gz'; 			sha256='fa5b6adfced2186a968fe36146e6103c4c6cc9aa849dfd1878644894eb28f0a7'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta1-linux-ppc64le.tar.gz'; 			sha256='8aa200030b6578334dcfc6404dbde8c894178b44d5eb88ec2b9bc8af8c8ce6e9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 16 Aug 2023 03:30:26 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 16 Aug 2023 03:30:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 03:30:27 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:41f92d5a73b9bee296c7b4a3817b28098b22fb60112608b42bb03570ca296115`  
		Last Modified: Tue, 15 Aug 2023 23:43:58 GMT  
		Size: 30.1 MB (30062816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10c589cedacd65337b5f6c97499d0435d181b4e1c1f7d2245aca9d5bb76f4466`  
		Last Modified: Wed, 16 Aug 2023 03:32:38 GMT  
		Size: 2.4 MB (2414400 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f38134e82057a010e4a0d224e5ebc0a481d97b0c368d87b974f7874e47f801ef`  
		Last Modified: Wed, 16 Aug 2023 03:32:57 GMT  
		Size: 161.6 MB (161606543 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c79a91719c679fdd4a864488bb457a72482d462605697a7be64a037e908cdd72`  
		Last Modified: Wed, 16 Aug 2023 03:32:37 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; 386

```console
$ docker pull julia@sha256:3f7ed7a6264ef9a13a668cec6df9939b2efd1152f7fee94e5f1e07d78a1117b5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.8 MB (188752000 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:99d0e620a0bdf5939f19476a54bf434098634101158baa7932aaa56587993f1c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 15 Aug 2023 23:39:23 GMT
ADD file:fa0abd37650f364ecdf67d446b3fe2ce58fac1ad53beb5263b4f230fad58931e in / 
# Tue, 15 Aug 2023 23:39:23 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 09:29:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 09:29:25 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 16 Aug 2023 09:29:26 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 09:29:26 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 16 Aug 2023 09:29:26 GMT
ENV JULIA_VERSION=1.10.0-beta1
# Wed, 16 Aug 2023 09:29:49 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta1-linux-x86_64.tar.gz'; 			sha256='cda38a2dd5b0ec605cc07ffa44efd3e9fe1072db26525953d1e24fb432e0bf4f'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta1-linux-aarch64.tar.gz'; 			sha256='e8377819ca383c7f4ee1841169625c578123244c592882d8706b5bf45f58ea37'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta1-linux-i686.tar.gz'; 			sha256='fa5b6adfced2186a968fe36146e6103c4c6cc9aa849dfd1878644894eb28f0a7'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta1-linux-ppc64le.tar.gz'; 			sha256='8aa200030b6578334dcfc6404dbde8c894178b44d5eb88ec2b9bc8af8c8ce6e9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 16 Aug 2023 09:29:52 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 16 Aug 2023 09:29:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 09:29:52 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:f6edc1df8dbb4cb778380e62ce1680ea580c1b213c048642bb7adaafa4cc6d73`  
		Last Modified: Tue, 15 Aug 2023 23:44:11 GMT  
		Size: 32.4 MB (32397200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:363daa537b5ac9e8288052a7c3caf6b4426146c870bd55aab53e5c234e5faba1`  
		Last Modified: Wed, 16 Aug 2023 09:32:58 GMT  
		Size: 2.5 MB (2532575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a7f0841c3bb0c703d6d573e3d0b7997630f6dab7e2f12a156a0eac7282cebe2`  
		Last Modified: Wed, 16 Aug 2023 09:33:29 GMT  
		Size: 153.8 MB (153821850 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7dcb9d457b781fad9b21bd4ccb373ea5011fcce00ee29639a3c161ae1be8f9a`  
		Last Modified: Wed, 16 Aug 2023 09:32:58 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `julia:rc-bullseye` - linux; ppc64le

```console
$ docker pull julia@sha256:3182eab564d3581c4fc879d22c0de940208f7d383d02889d5ad794103ec0fbd6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **188.9 MB (188946447 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1ed070ed8e4dcc606d8fb1b18b914b87d71b103598a343eecca6099feb8794d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Wed, 16 Aug 2023 01:10:12 GMT
ADD file:eeb766a3bb0461f0baa2425cfd43628994c064bd728f51f1b8df659a4bd2f489 in / 
# Wed, 16 Aug 2023 01:10:14 GMT
CMD ["bash"]
# Wed, 16 Aug 2023 03:49:50 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 16 Aug 2023 03:49:51 GMT
ENV JULIA_PATH=/usr/local/julia
# Wed, 16 Aug 2023 03:49:52 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 16 Aug 2023 03:49:52 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Wed, 16 Aug 2023 03:49:53 GMT
ENV JULIA_VERSION=1.10.0-beta1
# Wed, 16 Aug 2023 03:50:42 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta1-linux-x86_64.tar.gz'; 			sha256='cda38a2dd5b0ec605cc07ffa44efd3e9fe1072db26525953d1e24fb432e0bf4f'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta1-linux-aarch64.tar.gz'; 			sha256='e8377819ca383c7f4ee1841169625c578123244c592882d8706b5bf45f58ea37'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta1-linux-i686.tar.gz'; 			sha256='fa5b6adfced2186a968fe36146e6103c4c6cc9aa849dfd1878644894eb28f0a7'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta1-linux-ppc64le.tar.gz'; 			sha256='8aa200030b6578334dcfc6404dbde8c894178b44d5eb88ec2b9bc8af8c8ce6e9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version
# Wed, 16 Aug 2023 03:50:48 GMT
COPY file:92a2f9b3b9de38e57462f85dbe804b0eae9fea8a95aa9bfe9d3c2b95000ae42c in /usr/local/bin/ 
# Wed, 16 Aug 2023 03:50:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 16 Aug 2023 03:50:49 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:dacf4195c8a0403fd11459739bf9dc9be427261bf5e0bedb49e18d1498cf7c2e`  
		Last Modified: Wed, 16 Aug 2023 01:17:04 GMT  
		Size: 35.3 MB (35291067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e8c0ad3d55d5a63235dad071984f3be638dbc275fbe70e4917e5d0eef415eda`  
		Last Modified: Wed, 16 Aug 2023 03:54:46 GMT  
		Size: 2.6 MB (2627411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b0c9d9e3a8b9be06daf6976c96399a51fd175e056a10848699c0c0b6080f405`  
		Last Modified: Wed, 16 Aug 2023 03:55:25 GMT  
		Size: 151.0 MB (151027594 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2841f8ccdd0496adc6e36b78ae88e483a0548346349d1508fd6e12f547e000c6`  
		Last Modified: Wed, 16 Aug 2023 03:54:45 GMT  
		Size: 375.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
