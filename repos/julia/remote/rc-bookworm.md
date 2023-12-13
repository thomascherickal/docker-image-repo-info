## `julia:rc-bookworm`

```console
$ docker pull julia@sha256:76c8e9cc5bcb5218d6d8d33137823e82fac8ea8819154620530200a1a867cf22
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
$ docker pull julia@sha256:4b6e75045f534efc9f8bdbe15749a1ef1e23c7bafa55c85215df848a66e23003
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **206.2 MB (206199557 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5cde5945a039c5be2794241938e23acdd19361083f387c7994f1747d11503119`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 00:59:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 04 Dec 2023 00:59:15 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 04 Dec 2023 00:59:15 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 04 Dec 2023 00:59:15 GMT
ENV JULIA_VERSION=1.10.0-rc2
# Mon, 04 Dec 2023 00:59:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-rc2-linux-x86_64.tar.gz'; 			sha256='c1bf19a02758e6994aa292ed3fed047c6ff8d1cf433966a4848ad7facd01a6c5'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-rc2-linux-aarch64.tar.gz'; 			sha256='c2ad03382ba3a97558d6c6a8c028c48edc93e72fac71cb4368678fc92d8a8f4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-rc2-linux-i686.tar.gz'; 			sha256='e5fd504cc945d8685021e3d848acef132b98ce4352cef6b9ffacb30392055a4f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-rc2-linux-ppc64le.tar.gz'; 			sha256='edd3b75342f25f1a0059b839fd388adc433deb5c33c5af4a244426a7f73688c7'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.10.0-rc2","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.10.0-rc2?os_name=debian&os_version=bookworm"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 00:59:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:956c0bcb63520772ed4bcac217e9e7768cf77871397284bee7a82f77611d7cf4`  
		Last Modified: Tue, 05 Dec 2023 01:12:39 GMT  
		Size: 5.5 MB (5514480 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eb7acfa526d1b3871127f289a2e32dfb9447536e803d76f36ca173777b460b95`  
		Last Modified: Tue, 05 Dec 2023 01:12:42 GMT  
		Size: 171.5 MB (171534796 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:07ef4e1ea4a7b4c8de1ae2865820c132f7d752dfd4f398b6ad0ab73766cc80c1`  
		Last Modified: Tue, 05 Dec 2023 01:12:39 GMT  
		Size: 373.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bookworm` - unknown; unknown

```console
$ docker pull julia@sha256:fd8e179d3d29424cf1e2eedd9e3b0835a4fb3051ff2dcf46ad55218eab95fe9a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2120846 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5f1e9bd763d0376e602c6a1ac1792726c6d01f94e4a161609b84012e641534d1`

```dockerfile
```

-	Layers:
	-	`sha256:f50b7dca87de05c551641e2cfbbb236363c444ec4116c72c92747d86626ad5f4`  
		Last Modified: Tue, 05 Dec 2023 01:12:39 GMT  
		Size: 2.1 MB (2101977 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:deab8ae42d63db0a7251b94eaf604845552aa625612c0eb375df8a0fb4b21a77`  
		Last Modified: Tue, 05 Dec 2023 01:12:39 GMT  
		Size: 18.9 KB (18869 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:rc-bookworm` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:f66b22b91239e1ab07a604c4cc6f2b33627868a018453e820b97f9d510b163dc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **198.8 MB (198810387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b89ec4e2e570977abe61be6ef4f98e9ddc0e939d5ffbbefd66b70652fc551d7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 00:59:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 04 Dec 2023 00:59:15 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 04 Dec 2023 00:59:15 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 04 Dec 2023 00:59:15 GMT
ENV JULIA_VERSION=1.10.0-rc2
# Mon, 04 Dec 2023 00:59:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-rc2-linux-x86_64.tar.gz'; 			sha256='c1bf19a02758e6994aa292ed3fed047c6ff8d1cf433966a4848ad7facd01a6c5'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-rc2-linux-aarch64.tar.gz'; 			sha256='c2ad03382ba3a97558d6c6a8c028c48edc93e72fac71cb4368678fc92d8a8f4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-rc2-linux-i686.tar.gz'; 			sha256='e5fd504cc945d8685021e3d848acef132b98ce4352cef6b9ffacb30392055a4f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-rc2-linux-ppc64le.tar.gz'; 			sha256='edd3b75342f25f1a0059b839fd388adc433deb5c33c5af4a244426a7f73688c7'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.10.0-rc2","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.10.0-rc2?os_name=debian&os_version=bookworm"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 00:59:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b3b7cabcb5585cb7d4dc21464688cea29a3ae6f2f1367ac8cad3058362866ea`  
		Last Modified: Tue, 05 Dec 2023 01:30:48 GMT  
		Size: 5.3 MB (5339542 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2b6fce37b449980a8a429682cdccd08a20bb99dc7620f55bd4edf8f77345f94b`  
		Last Modified: Tue, 05 Dec 2023 01:30:53 GMT  
		Size: 164.3 MB (164291197 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f67b4d882c79ab8e29d7215a6a94ae1fe0e2ef65b35c38fdb6399eea5b98b8eb`  
		Last Modified: Tue, 05 Dec 2023 01:30:47 GMT  
		Size: 371.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bookworm` - unknown; unknown

```console
$ docker pull julia@sha256:cf67ea118e7b1a20143f2e943430916a45ecb5f05040a19ad1bad2425561e9c6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2121032 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8a5847ca49573f04ef0569c3417a33d1b2906eac7d197289a82f69abdd020fdf`

```dockerfile
```

-	Layers:
	-	`sha256:83cd2ed1fa7c729e8922c2472124708c0137af220a67e6355dd481aaf4f781b2`  
		Last Modified: Tue, 05 Dec 2023 01:30:48 GMT  
		Size: 2.1 MB (2102316 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:06ca17c60007e6bf5fb06b2281f267d8d8a3bac72558c0aa2759aaebf978596d`  
		Last Modified: Tue, 05 Dec 2023 01:30:47 GMT  
		Size: 18.7 KB (18716 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:rc-bookworm` - linux; 386

```console
$ docker pull julia@sha256:4367799884c0e0f19ec08b99b28271cb1f7f35486a85cee072a42be1d65afc54
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **192.2 MB (192188721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aeffe3452a298b7129c7b452e710b96fc4d265f2635ce42b347cc9061262061d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Nov 2023 04:39:53 GMT
ADD file:930e1b9d85b6927c4d3046f7c75de2f3bfc6ec29100c314d0ab2b780ea30e962 in / 
# Tue, 21 Nov 2023 04:39:53 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 00:59:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 04 Dec 2023 00:59:15 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 04 Dec 2023 00:59:15 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 04 Dec 2023 00:59:15 GMT
ENV JULIA_VERSION=1.10.0-rc2
# Mon, 04 Dec 2023 00:59:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-rc2-linux-x86_64.tar.gz'; 			sha256='c1bf19a02758e6994aa292ed3fed047c6ff8d1cf433966a4848ad7facd01a6c5'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-rc2-linux-aarch64.tar.gz'; 			sha256='c2ad03382ba3a97558d6c6a8c028c48edc93e72fac71cb4368678fc92d8a8f4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-rc2-linux-i686.tar.gz'; 			sha256='e5fd504cc945d8685021e3d848acef132b98ce4352cef6b9ffacb30392055a4f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-rc2-linux-ppc64le.tar.gz'; 			sha256='edd3b75342f25f1a0059b839fd388adc433deb5c33c5af4a244426a7f73688c7'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.10.0-rc2","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.10.0-rc2?os_name=debian&os_version=bookworm"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 00:59:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c0734eabce8885d8904dbd11b77aa97c2d2b04bc8e2af9e89d47c4bda590dd8e`  
		Last Modified: Tue, 21 Nov 2023 04:44:34 GMT  
		Size: 30.2 MB (30164109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b69b936b9b06e9c52e214455e3bfd37c86a2893adf558d8d607c321e24b7f2fa`  
		Last Modified: Tue, 05 Dec 2023 01:12:30 GMT  
		Size: 5.7 MB (5671156 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e37e619ce62957d006cfe08d3741cc7fab6bc0c37e74b5b6d2647a237241d7ea`  
		Last Modified: Tue, 05 Dec 2023 01:12:34 GMT  
		Size: 156.4 MB (156353088 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d4726765a5f4b83d5f2bd062f96c1faeecdab842ff684111bd5a1273179806bc`  
		Last Modified: Tue, 05 Dec 2023 01:12:30 GMT  
		Size: 368.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bookworm` - unknown; unknown

```console
$ docker pull julia@sha256:24ffb0e0129adc087bf0a66f3aa8c870ffadfaf700f96515171b8f2e665810d1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **18.6 KB (18613 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13306ed1be436a497d8a890b49b77b9a7f5386ee32f412e796bbf03f92b65dde`

```dockerfile
```

-	Layers:
	-	`sha256:fce7d6c517378ab6c4ef2390a3f644bfebc7cd549f362c8ced99aa66e1d5e68f`  
		Last Modified: Tue, 05 Dec 2023 01:12:30 GMT  
		Size: 18.6 KB (18613 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:rc-bookworm` - linux; ppc64le

```console
$ docker pull julia@sha256:829d143f55d447e297afbdf490edc55fb0ff4e5d6ac9b3da1560c937302d473e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **193.3 MB (193349588 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8e66de1d136d35dc1520cc2661d36d5b789b30c14b6c971c63dffc47586df858`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:14 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Tue, 21 Nov 2023 04:24:16 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 00:59:15 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 04 Dec 2023 00:59:15 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 04 Dec 2023 00:59:15 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 04 Dec 2023 00:59:15 GMT
ENV JULIA_VERSION=1.10.0-rc2
# Mon, 04 Dec 2023 00:59:15 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-rc2-linux-x86_64.tar.gz'; 			sha256='c1bf19a02758e6994aa292ed3fed047c6ff8d1cf433966a4848ad7facd01a6c5'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-rc2-linux-aarch64.tar.gz'; 			sha256='c2ad03382ba3a97558d6c6a8c028c48edc93e72fac71cb4368678fc92d8a8f4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-rc2-linux-i686.tar.gz'; 			sha256='e5fd504cc945d8685021e3d848acef132b98ce4352cef6b9ffacb30392055a4f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-rc2-linux-ppc64le.tar.gz'; 			sha256='edd3b75342f25f1a0059b839fd388adc433deb5c33c5af4a244426a7f73688c7'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.10.0-rc2","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.10.0-rc2?os_name=debian&os_version=bookworm"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 00:59:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b62138e786d628f38698517c1db5da7a943cf4eb936faca501877c4d8e4a1892`  
		Last Modified: Tue, 05 Dec 2023 01:15:34 GMT  
		Size: 6.0 MB (6046525 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:db7078ed1e521aaa040e01ec20ecd0f26b36d75c7fcfadcb7d2c2818f93e21cd`  
		Last Modified: Tue, 05 Dec 2023 01:15:38 GMT  
		Size: 154.2 MB (154161087 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3570f8154687ec1da5ccb02ffc4080f841780923ed7c136d0d7a4c2980a7d755`  
		Last Modified: Tue, 05 Dec 2023 01:15:34 GMT  
		Size: 369.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bookworm` - unknown; unknown

```console
$ docker pull julia@sha256:64f3636fef788c3c376f0b6f984101ade0b42c397f3988ee2cfa0e48722fa055
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.1 MB (2125256 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:35369f8a7389aa925a2501d44758c871a97768dfb925a1b670beccbd52200ed4`

```dockerfile
```

-	Layers:
	-	`sha256:e0a60cf9f4c6dbe56334d18106ed5b97bbb87321e35c67b5d2cb0a4a4d365f3d`  
		Last Modified: Tue, 05 Dec 2023 01:15:34 GMT  
		Size: 2.1 MB (2106502 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:db0da1590f6b7d0fb253bd578453bb5a37ba254225546f250ed425073bbb09a2`  
		Last Modified: Tue, 05 Dec 2023 01:15:34 GMT  
		Size: 18.8 KB (18754 bytes)  
		MIME: application/vnd.in-toto+json
