## `julia:rc-bullseye`

```console
$ docker pull julia@sha256:5213a1b2dc50cce17cd94f4e551925165051201bcfedf93611b6fd8feca5b880
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

### `julia:rc-bullseye` - linux; amd64

```console
$ docker pull julia@sha256:a4e1fda2dea27a5512fa1508b4a0f74af275692ead16d851fd2cc0a4f70adb7c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **204.9 MB (204915244 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:335c15fb171ea2fa5bcde05e3165f477441a9c145016ccc2a6c84fd403ad01c3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Mon, 18 Dec 2023 21:28:57 GMT
ADD file:bb44d67b03db8efaeb0c4171474f441d14ff35f328f13add32b289fca062fa2f in / 
# Mon, 18 Dec 2023 21:28:57 GMT
CMD ["bash"]
# Mon, 18 Dec 2023 21:28:57 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 18 Dec 2023 21:28:57 GMT
ENV JULIA_PATH=/usr/local/julia
# Mon, 18 Dec 2023 21:28:57 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Mon, 18 Dec 2023 21:28:57 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Mon, 18 Dec 2023 21:28:57 GMT
ENV JULIA_VERSION=1.10.0-rc3
# Mon, 18 Dec 2023 21:28:57 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-rc3-linux-x86_64.tar.gz'; 			sha256='cb68ef2ebff2cfd18c1cba2c1ad8f37e73685ae6a24dbc036dfc86b2e13e0a18'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-rc3-linux-aarch64.tar.gz'; 			sha256='dc0baea6e9a7a1ec608b641d0658f1621a471b602b13a0facb72e0b83ccc8e6d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-rc3-linux-i686.tar.gz'; 			sha256='ac6938aab1d824029bf60959f80c3da7bbb5660aa32e9e97a5f7269a5c5c3986'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-rc3-linux-ppc64le.tar.gz'; 			sha256='45a499f7de8fabe5321469d3912a1b9bcddc15b3ddcc6c1671a5754f36a0e2e9'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.10.0-rc3","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.10.0-rc3?os_name=debian&os_version=bullseye"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Mon, 18 Dec 2023 21:28:57 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 18 Dec 2023 21:28:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 18 Dec 2023 21:28:57 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b5a0d5c14ba9ece1eecd5137c468d9a123372b0af2ed2c8c4446137730c90e5b`  
		Last Modified: Tue, 19 Dec 2023 01:25:40 GMT  
		Size: 31.4 MB (31417873 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:57cd27c8af6717c71945ed6af9eddd5c2a0b54c0b7669dd1c0fb8a90f5db2417`  
		Last Modified: Tue, 19 Dec 2023 03:48:04 GMT  
		Size: 2.2 MB (2223255 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:62e63124db438f7a06b92ba3b41c732911f51a5a8a9865a34b62d88eac0d2c4f`  
		Last Modified: Tue, 19 Dec 2023 03:48:08 GMT  
		Size: 171.3 MB (171273746 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:00973b6d28b6851e9f49ac29e8ec43d6e79d9ac1ca6d4945e6c5838de1e598f6`  
		Last Modified: Tue, 19 Dec 2023 03:48:04 GMT  
		Size: 370.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bullseye` - unknown; unknown

```console
$ docker pull julia@sha256:7967677a6897aa46257c6b3258dc9f7fdf1ad59e251ce4292a5abe436095082c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 MB (2249104 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8204e590ed03487ef4b7cb8cfdeb32f5dd8c63b8aa4695bac1a7e55125e45955`

```dockerfile
```

-	Layers:
	-	`sha256:300b94fc83182999fbfe317205bd80f34605c3c3e7f4e424d93f9b583b555ad9`  
		Last Modified: Tue, 19 Dec 2023 03:48:04 GMT  
		Size: 2.2 MB (2231125 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:01f9f22d2e01722c2af922cb7f7840d67aac1d90312e89bf0e168452dd9c0fff`  
		Last Modified: Tue, 19 Dec 2023 03:48:04 GMT  
		Size: 18.0 KB (17979 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:rc-bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:e8c0719a461d89ff26c4aa6e8f5b4993fedc364a13af24b237292c2980c5d896
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **196.6 MB (196567596 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d37b91207cf305277fb141135b1717a8d8cbadf902328d38c83b9af564c9839`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:20 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 21 Nov 2023 06:27:21 GMT
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
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-rc2-linux-x86_64.tar.gz'; 			sha256='c1bf19a02758e6994aa292ed3fed047c6ff8d1cf433966a4848ad7facd01a6c5'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-rc2-linux-aarch64.tar.gz'; 			sha256='c2ad03382ba3a97558d6c6a8c028c48edc93e72fac71cb4368678fc92d8a8f4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-rc2-linux-i686.tar.gz'; 			sha256='e5fd504cc945d8685021e3d848acef132b98ce4352cef6b9ffacb30392055a4f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-rc2-linux-ppc64le.tar.gz'; 			sha256='edd3b75342f25f1a0059b839fd388adc433deb5c33c5af4a244426a7f73688c7'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.10.0-rc2","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.10.0-rc2?os_name=debian&os_version=bullseye"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 00:59:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:7ca1f7b92c8362fe2a968882ca38e77971fb5136f1582283b8655b5788e51322`  
		Last Modified: Tue, 05 Dec 2023 01:31:53 GMT  
		Size: 2.2 MB (2211126 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ca96c2db6586af1fe2e2a7506089bff6052cb169e01f92b1566afa9bd7707b88`  
		Last Modified: Tue, 05 Dec 2023 01:31:57 GMT  
		Size: 164.3 MB (164291976 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a14d62d57f650db2608615c3a279df42072d6a92a363fce8d4f516403abbba24`  
		Last Modified: Tue, 05 Dec 2023 01:31:52 GMT  
		Size: 371.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bullseye` - unknown; unknown

```console
$ docker pull julia@sha256:4d5b9c920f1911580862a39ee6b8881a371299cf40c1038ca2333623cbbffdbf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 MB (2249268 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b57964bf6a9513f8c97252e514d6b6cfb5272a87448dbdf9be4eedee822a348`

```dockerfile
```

-	Layers:
	-	`sha256:e248c042c2768f39e61e835684fa4b16c2751b642e843bc35f31d8c6ec84b0f7`  
		Last Modified: Tue, 05 Dec 2023 01:31:53 GMT  
		Size: 2.2 MB (2231448 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:59d3876952193b67023c6b76a9a05c5ec8aaa790e3b7f4d8f2800815a56bafd6`  
		Last Modified: Tue, 05 Dec 2023 01:31:53 GMT  
		Size: 17.8 KB (17820 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:rc-bullseye` - linux; 386

```console
$ docker pull julia@sha256:6f57981fc2555b2f317aa3078d8fb9057d755a4efd24609825742ead367dcf74
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.1 MB (191086723 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3b0a1747c423a5620b38c937137d9fbb4a41a4e9215a603eb9f585010f6bcfab`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Nov 2023 04:40:15 GMT
ADD file:7de881b584405a880c4d02778056aaa81bb5dd5d1af65b3086d66aed9ff0ad4b in / 
# Tue, 21 Nov 2023 04:40:16 GMT
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
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-rc2-linux-x86_64.tar.gz'; 			sha256='c1bf19a02758e6994aa292ed3fed047c6ff8d1cf433966a4848ad7facd01a6c5'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-rc2-linux-aarch64.tar.gz'; 			sha256='c2ad03382ba3a97558d6c6a8c028c48edc93e72fac71cb4368678fc92d8a8f4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-rc2-linux-i686.tar.gz'; 			sha256='e5fd504cc945d8685021e3d848acef132b98ce4352cef6b9ffacb30392055a4f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-rc2-linux-ppc64le.tar.gz'; 			sha256='edd3b75342f25f1a0059b839fd388adc433deb5c33c5af4a244426a7f73688c7'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.10.0-rc2","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.10.0-rc2?os_name=debian&os_version=bullseye"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 00:59:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:75c11612678b54e79a38118fe66e532c61b3d0798afb741007b4cd3209c0ec4e`  
		Last Modified: Tue, 21 Nov 2023 04:45:24 GMT  
		Size: 32.4 MB (32402632 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0e7d7ed948db8d0b9c5df8fe93b5e8fff475d07b44b6a1af07ea9854d1aa5bd7`  
		Last Modified: Tue, 05 Dec 2023 01:12:41 GMT  
		Size: 2.3 MB (2328963 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:238d1758410207775b302979241f9140963a041923575cfb341eb7070c0ab633`  
		Last Modified: Tue, 05 Dec 2023 01:12:46 GMT  
		Size: 156.4 MB (156354758 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:d6886b47342128b174a295d5a1aae031083a6fecfc6b821010e559958e3d6aae`  
		Last Modified: Tue, 05 Dec 2023 01:12:41 GMT  
		Size: 370.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bullseye` - unknown; unknown

```console
$ docker pull julia@sha256:d6da8ffae6fc32b4a6199c39b0d29725e7b5d21d2c3265be43d1513a929884f0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.7 KB (17738 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9243044179093b1e1c5a47bd42aee90396dae7e51520cf7f9d846baaf4cdfa85`

```dockerfile
```

-	Layers:
	-	`sha256:3422cbdc62fbb79b736c17f624ad4b1f15d466ea8d7144167637c3f5d5fc952c`  
		Last Modified: Tue, 05 Dec 2023 01:12:40 GMT  
		Size: 17.7 KB (17738 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:rc-bullseye` - linux; ppc64le

```console
$ docker pull julia@sha256:c5f0aae819a23831f246a5f1f1a7c6bd640356f428285a4089b1f9abeb6c0ed4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **191.9 MB (191881129 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f8ce1a0b288bcf59cc2879eec85507ac01bc98a0c0d1ec7a394bca907606f018`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 21 Nov 2023 04:24:43 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 21 Nov 2023 04:24:46 GMT
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
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.10/julia-1.10.0-rc2-linux-x86_64.tar.gz'; 			sha256='c1bf19a02758e6994aa292ed3fed047c6ff8d1cf433966a4848ad7facd01a6c5'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.10/julia-1.10.0-rc2-linux-aarch64.tar.gz'; 			sha256='c2ad03382ba3a97558d6c6a8c028c48edc93e72fac71cb4368678fc92d8a8f4d'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.10/julia-1.10.0-rc2-linux-i686.tar.gz'; 			sha256='e5fd504cc945d8685021e3d848acef132b98ce4352cef6b9ffacb30392055a4f'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.10/julia-1.10.0-rc2-linux-ppc64le.tar.gz'; 			sha256='edd3b75342f25f1a0059b839fd388adc433deb5c33c5af4a244426a7f73688c7'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.10.0-rc2","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.10.0-rc2?os_name=debian&os_version=bullseye"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 00:59:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 00:59:15 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:30b11a4f6a3cb618be823cff821cf8a1813b07e058843920991dc9be398ff1f9`  
		Last Modified: Tue, 05 Dec 2023 01:18:59 GMT  
		Size: 2.4 MB (2425658 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:98fa24b32c3cb0894a470d79dbe1aeb882e0be6afe704b50782532de881ecd51`  
		Last Modified: Tue, 05 Dec 2023 01:19:03 GMT  
		Size: 154.2 MB (154161368 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2e54075babd93a69de098eb71efc95a8e1e553f9f0ee39ea0b3f06a47ce838be`  
		Last Modified: Tue, 05 Dec 2023 01:18:58 GMT  
		Size: 376.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:rc-bullseye` - unknown; unknown

```console
$ docker pull julia@sha256:f2d0c4d3f4a8301cacab8be79fc0defc093022b0b562a318eb60e5e55009f9b6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 MB (2253468 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a10b4df934df9cc919f5de5de29c9a52d7440a311852955fc055a7c8e628e9f9`

```dockerfile
```

-	Layers:
	-	`sha256:2ddb70fd4d86d94a6513e97a2e22b670e648c94cfa006e7f382bdd1817ccf337`  
		Last Modified: Tue, 05 Dec 2023 01:18:59 GMT  
		Size: 2.2 MB (2235622 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:2b08392c72ceb84de694abf46f0e99e2ddae5fa45645c22f7596e31cf8e78e15`  
		Last Modified: Tue, 05 Dec 2023 01:18:59 GMT  
		Size: 17.8 KB (17846 bytes)  
		MIME: application/vnd.in-toto+json
