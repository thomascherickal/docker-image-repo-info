## `julia:rc-bookworm`

```console
$ docker pull julia@sha256:3a2cb9e6a05898f30dcb75dbcf07b0dc00ef97df2291fdce645b3a01a80d1f43
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 8
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown

### `julia:rc-bookworm` - linux; amd64

```console
$ docker pull julia@sha256:6396b48924f623b735b70dfd4b84609c413536530ab083416a80abf11d369a0f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.5 MB (204500164 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a55ae584a22347ed5af534bedfdc9f3316302fc2faf19156d35474b49c099b51`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 03 Oct 2023 23:59:11 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Tue, 03 Oct 2023 23:59:11 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 23:59:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 23:59:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 03 Oct 2023 23:59:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:59:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 03 Oct 2023 23:59:11 GMT
ENV JULIA_VERSION=1.10.0-beta3
# Tue, 03 Oct 2023 23:59:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta3-linux-x86_64.tar.gz'; 			sha256='f6fb0b8625f608c6b586f96e6f403da827c5f69ee0fa72746e0c3b5b6eb29022'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta3-linux-aarch64.tar.gz'; 			sha256='9ee2d8ff367f17efa7d7279415622d85ae3e592a0938cc2c90a41f6d6f5a28d2'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta3-linux-i686.tar.gz'; 			sha256='2a18c67f4b3222018b74c5fc0d0c2211784fbd4905c43b55fa714b774b941614'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta3-linux-ppc64le.tar.gz'; 			sha256='40c541540f610736813750017ddc7292067438190a1a78ba30604abcd2bc4818'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version # buildkit
# Tue, 03 Oct 2023 23:59:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 03 Oct 2023 23:59:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Oct 2023 23:59:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6985ca9979715b96fcd868f241348000d5f93101c4bf873801192c8e09966020`  
		Last Modified: Fri, 20 Oct 2023 16:03:02 GMT  
		Size: 5.5 MB (5513800 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f8e938b3af6f7ddbe7326fc5159be506f55ca14f101bc6be3beee2bba3319e59`  
		Last Modified: Fri, 20 Oct 2023 16:03:12 GMT  
		Size: 169.8 MB (169836120 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:cd23cd03fe35ea3551a9e637ae666539099e83785eac996b338cfe7a2e84bdb6`  
		Last Modified: Fri, 20 Oct 2023 16:03:02 GMT  
		Size: 370.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bookworm` - unknown; unknown

```console
$ docker pull julia@sha256:5c9a0a65594f9e76f15f831c67f4ae8a4e5ef5281751c6b05990e67a2208101a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2118769 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:30cbe5b0118b4b525f758e16b9d8dae2ee8161d5b619fd5a5be03acc0379ee3d`

```dockerfile
```

-	Layers:
	-	`sha256:3ba878958bc45f46ffc8aacdd96f8f83d0714a8f31d1a4fe6c87cd4c4ca0f49b`  
		Last Modified: Fri, 20 Oct 2023 16:03:03 GMT  
		Size: 2.1 MB (2100930 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9484e01054a0023e9e89b768b7c8a03002dc9a71de70acec501fb42c6c00ee87`  
		Last Modified: Fri, 20 Oct 2023 16:03:02 GMT  
		Size: 17.8 KB (17839 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:rc-bookworm` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:19ce9e214809d9f7b8b1571b8d9437b1514b7707f5792f457beaf1f58eda12e1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **199.1 MB (199051343 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d25573dd93aa707a18683efee7e8c77d5132dbf572d275a5515f6fb30a78dba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 03 Oct 2023 23:59:11 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Tue, 03 Oct 2023 23:59:11 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 23:59:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 23:59:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 03 Oct 2023 23:59:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:59:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 03 Oct 2023 23:59:11 GMT
ENV JULIA_VERSION=1.10.0-beta3
# Tue, 03 Oct 2023 23:59:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta3-linux-x86_64.tar.gz'; 			sha256='f6fb0b8625f608c6b586f96e6f403da827c5f69ee0fa72746e0c3b5b6eb29022'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta3-linux-aarch64.tar.gz'; 			sha256='9ee2d8ff367f17efa7d7279415622d85ae3e592a0938cc2c90a41f6d6f5a28d2'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta3-linux-i686.tar.gz'; 			sha256='2a18c67f4b3222018b74c5fc0d0c2211784fbd4905c43b55fa714b774b941614'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta3-linux-ppc64le.tar.gz'; 			sha256='40c541540f610736813750017ddc7292067438190a1a78ba30604abcd2bc4818'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version # buildkit
# Tue, 03 Oct 2023 23:59:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 03 Oct 2023 23:59:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Oct 2023 23:59:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:59cc0860576145b9aba41c89910507f1614704d3d427324ef415d234c50c70a1`  
		Last Modified: Fri, 20 Oct 2023 20:13:02 GMT  
		Size: 5.3 MB (5338906 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5a14311dc190efd081b128b52d319a52587947697a0de91ba33a79dfc29443f7`  
		Last Modified: Fri, 20 Oct 2023 20:13:10 GMT  
		Size: 164.5 MB (164532784 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f512ad710af4ee1f931c77650236e9344d19cb3c261a6ae68e0be630e1cace13`  
		Last Modified: Fri, 20 Oct 2023 20:13:01 GMT  
		Size: 369.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bookworm` - unknown; unknown

```console
$ docker pull julia@sha256:9e8d3fa84a1e3b2386baa4b80fc57c593336e37307d88cdb97226f2a735a2b58
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2118955 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:58dc5ef84a2ecbbf2d7c84abe01bf18e6563c3971a57dd7779ea8f27e0394317`

```dockerfile
```

-	Layers:
	-	`sha256:22eead1475d0cd92778dacd79428850af24fa4e52be46457128b039a8a261c9b`  
		Last Modified: Fri, 20 Oct 2023 20:13:02 GMT  
		Size: 2.1 MB (2101269 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d99b1097c81da7f938f95bfa953c2c7e6ff10e1f3e8043f007c1cdd028c493a7`  
		Last Modified: Fri, 20 Oct 2023 20:13:01 GMT  
		Size: 17.7 KB (17686 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:rc-bookworm` - linux; 386

```console
$ docker pull julia@sha256:78ae509ab2a72be2e413c7c1ed9ad1e65078670820fa642dc4239be14c90ef63
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.3 MB (192336779 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83e5376a6d4533ff5ba2418b33e2ff6a24b73032862ac540e20021d342bc6ace`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 03 Oct 2023 23:59:11 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Tue, 03 Oct 2023 23:59:11 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 23:59:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 23:59:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 03 Oct 2023 23:59:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:59:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 03 Oct 2023 23:59:11 GMT
ENV JULIA_VERSION=1.10.0-beta3
# Tue, 03 Oct 2023 23:59:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta3-linux-x86_64.tar.gz'; 			sha256='f6fb0b8625f608c6b586f96e6f403da827c5f69ee0fa72746e0c3b5b6eb29022'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta3-linux-aarch64.tar.gz'; 			sha256='9ee2d8ff367f17efa7d7279415622d85ae3e592a0938cc2c90a41f6d6f5a28d2'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta3-linux-i686.tar.gz'; 			sha256='2a18c67f4b3222018b74c5fc0d0c2211784fbd4905c43b55fa714b774b941614'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta3-linux-ppc64le.tar.gz'; 			sha256='40c541540f610736813750017ddc7292067438190a1a78ba30604abcd2bc4818'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version # buildkit
# Tue, 03 Oct 2023 23:59:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 03 Oct 2023 23:59:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Oct 2023 23:59:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e5d176cc6b2c9720ccfe720dd97d08f32bbc3f108cc7a3492f4f9b809e35ba97`  
		Last Modified: Wed, 01 Nov 2023 02:08:34 GMT  
		Size: 5.7 MB (5669665 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2947787a2287f3be341f4e681e307f11466714f9ff7ec1d0c092340d70cb30e5`  
		Last Modified: Wed, 01 Nov 2023 02:08:42 GMT  
		Size: 156.5 MB (156502702 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:719cc53cef2eea3fca35be1dcc010a8a2604e80ee0b5bf49b60729d6fd7617f5`  
		Last Modified: Wed, 01 Nov 2023 02:08:34 GMT  
		Size: 370.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bookworm` - unknown; unknown

```console
$ docker pull julia@sha256:1e50dc1f219f824f96f4ade466a07f5615afd9fad6a87bdb8f36cce50dcdd0ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.6 KB (17583 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cd1a5063206eb51eb64dd125a781215adb7d97ecac897451a9565697b847df4e`

```dockerfile
```

-	Layers:
	-	`sha256:a08936c387e76a2893b8d93b89587a366aae3bb9ddf302abb0942651901432d6`  
		Last Modified: Wed, 01 Nov 2023 02:08:34 GMT  
		Size: 17.6 KB (17583 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:rc-bookworm` - linux; ppc64le

```console
$ docker pull julia@sha256:1e4bd653f031a1e7e2bd53c8caf8f276a6073a53fe01d3c0f0f6f92aa14f0003
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.0 MB (193019258 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:db416bc9b98adec468e8bc4ddb051a7ef3b1bf0282526324dbff94fb23d0cd3f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 03 Oct 2023 23:59:11 GMT
ADD file:f36d600ab8508979b5763875a75f35555fa0a83d2656cbcdfa50978c6ae97353 in / 
# Tue, 03 Oct 2023 23:59:11 GMT
CMD ["bash"]
# Tue, 03 Oct 2023 23:59:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 03 Oct 2023 23:59:11 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 03 Oct 2023 23:59:11 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 03 Oct 2023 23:59:11 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 03 Oct 2023 23:59:11 GMT
ENV JULIA_VERSION=1.10.0-beta3
# Tue, 03 Oct 2023 23:59:11 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-beta3-linux-x86_64.tar.gz'; 			sha256='f6fb0b8625f608c6b586f96e6f403da827c5f69ee0fa72746e0c3b5b6eb29022'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-beta3-linux-aarch64.tar.gz'; 			sha256='9ee2d8ff367f17efa7d7279415622d85ae3e592a0938cc2c90a41f6d6f5a28d2'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-beta3-linux-i686.tar.gz'; 			sha256='2a18c67f4b3222018b74c5fc0d0c2211784fbd4905c43b55fa714b774b941614'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-beta3-linux-ppc64le.tar.gz'; 			sha256='40c541540f610736813750017ddc7292067438190a1a78ba30604abcd2bc4818'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version # buildkit
# Tue, 03 Oct 2023 23:59:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 03 Oct 2023 23:59:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 03 Oct 2023 23:59:11 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:e56c8f20d7d119ff87eb044f21bfd5a4b30bf8436fc5fac12871095a6bd1517c`  
		Last Modified: Wed, 01 Nov 2023 00:26:10 GMT  
		Size: 33.1 MB (33141482 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:731fefc00fefcf2648725a405996c24f3f813cefde0845d8a9540eb613b297f1`  
		Last Modified: Wed, 01 Nov 2023 13:51:05 GMT  
		Size: 6.0 MB (6045806 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ac41f37462d57ae6530dca0a3115d78f0fcd1d244fa2ce0712c55e658bc9f67d`  
		Last Modified: Wed, 01 Nov 2023 13:51:15 GMT  
		Size: 153.8 MB (153831594 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6f311f19b9898e6ce46661f097aa594090f5486cea2bcbd995127c30777eca81`  
		Last Modified: Wed, 01 Nov 2023 13:51:04 GMT  
		Size: 376.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bookworm` - unknown; unknown

```console
$ docker pull julia@sha256:923dc601cb6668682e8697416b6f39ca495a19483de2b9965770a22a8b4bb7c3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2123345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dee703b0d121dd68e4614d8d99d967fd73aa09b4e084249d1546adcce18f4c7f`

```dockerfile
```

-	Layers:
	-	`sha256:9ccd3c63f34bdd7246ec8f335d847f568932a8b337d407ee48a67914316aeb38`  
		Last Modified: Wed, 01 Nov 2023 13:51:04 GMT  
		Size: 2.1 MB (2105455 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:7255f70fc49d7298f2717008f4875a7a892433cd59513668fca0ff3ea73fe9ed`  
		Last Modified: Wed, 01 Nov 2023 13:51:04 GMT  
		Size: 17.9 KB (17890 bytes)  
		MIME: application/vnd.in-toto+json
