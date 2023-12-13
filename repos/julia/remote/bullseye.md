## `julia:bullseye`

```console
$ docker pull julia@sha256:611bee55b931d57fda8e2146ee3d3242b2d651ee4344167c7a5f7c3d5c847629
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

### `julia:bullseye` - linux; amd64

```console
$ docker pull julia@sha256:dfc6902bc211ad113004c3b57a6483a66d86f370980e1feee7035b70c056a09f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **182.2 MB (182215231 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3ff9786d3d80e04f48a1437d234a6c461dc4bda6747ccb747e303bb4f52dc663`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 14 Nov 2023 18:59:25 GMT
ADD file:e9f63d1defc55282fec6525ac2886c735dc2189e34105d7fe64c2420d6673922 in / 
# Tue, 14 Nov 2023 18:59:25 GMT
CMD ["bash"]
# Tue, 14 Nov 2023 18:59:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 14 Nov 2023 18:59:25 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_VERSION=1.9.4
# Tue, 14 Nov 2023 18:59:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.4-linux-x86_64.tar.gz'; 			sha256='07d20c4c2518833e2265ca0acee15b355463361aa4efdab858dad826cf94325c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.4-linux-aarch64.tar.gz'; 			sha256='541d0c5a9378f8d2fc384bb8595fc6ffe20d61054629a6e314fb2f8dfe2f2ade'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.4-linux-i686.tar.gz'; 			sha256='2b045a30c6ed8b14a5f4b7ecfb74ef2af7d70b85c9b513cd347886c8dace39bd'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.4-linux-ppc64le.tar.gz'; 			sha256='a5da86c0f0f4ef6d8645f74d8397a6e833831ee212de9edc52e4aefe8f368494'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.9.4","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.9.4?os_name=debian&os_version=bullseye"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Nov 2023 18:59:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:b7f91549542cca4b35a34cdee5364339f17468971ea730bb072864d3e78c8b94`  
		Last Modified: Tue, 21 Nov 2023 05:26:39 GMT  
		Size: 31.4 MB (31417824 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a5a9cdddb43fca6bac983b11e5645e8265787249b836985ebe5c116c2ac9c15`  
		Last Modified: Tue, 21 Nov 2023 06:17:04 GMT  
		Size: 2.2 MB (2222786 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a710f61b516f3f4787796923acd99f6139480efddcb6e163557961deace760bc`  
		Last Modified: Tue, 21 Nov 2023 06:17:06 GMT  
		Size: 148.6 MB (148574253 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2a435ad69b62cea8213cb59fc2affe7d8d565a311d9a488ad3b8217a933c0927`  
		Last Modified: Tue, 21 Nov 2023 06:16:55 GMT  
		Size: 368.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:bullseye` - unknown; unknown

```console
$ docker pull julia@sha256:7a7f65b7685bed34c5ca903c45ef513e251af3b20e32150e2e2e036b266c1686
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 MB (2249515 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:620af297869db04a0989d208833ddf7c65172c3f066dfb0ee60e063c31a01bef`

```dockerfile
```

-	Layers:
	-	`sha256:dd8882f27403a04f3dee58859078529c51ca5a0ebe596da83f365df5af167084`  
		Last Modified: Tue, 21 Nov 2023 06:17:03 GMT  
		Size: 2.2 MB (2231363 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:97639b2a57be0688aa01a91e92d86dff612a8855e40c0d5db4023b3bd9a33538`  
		Last Modified: Tue, 21 Nov 2023 06:17:03 GMT  
		Size: 18.2 KB (18152 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:bullseye` - linux; arm64 variant v8

```console
$ docker pull julia@sha256:e93d5fd6ff2948c8cff1b98829e580a576ad28b018f217ced6083211fa18e344
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **175.0 MB (175006550 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:430eef67f16dd22475f93edc2c2f16b9c1aa19fcc43feb9e3d1001ac5485762d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 14 Nov 2023 18:59:25 GMT
ADD file:7b5bbc3b85f671aaf7b38dbe3fc76aae162bbff29c525bcd127f8a26a53bc664 in / 
# Tue, 14 Nov 2023 18:59:25 GMT
CMD ["bash"]
# Tue, 14 Nov 2023 18:59:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 14 Nov 2023 18:59:25 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_VERSION=1.9.4
# Tue, 14 Nov 2023 18:59:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.4-linux-x86_64.tar.gz'; 			sha256='07d20c4c2518833e2265ca0acee15b355463361aa4efdab858dad826cf94325c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.4-linux-aarch64.tar.gz'; 			sha256='541d0c5a9378f8d2fc384bb8595fc6ffe20d61054629a6e314fb2f8dfe2f2ade'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.4-linux-i686.tar.gz'; 			sha256='2b045a30c6ed8b14a5f4b7ecfb74ef2af7d70b85c9b513cd347886c8dace39bd'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.4-linux-ppc64le.tar.gz'; 			sha256='a5da86c0f0f4ef6d8645f74d8397a6e833831ee212de9edc52e4aefe8f368494'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.9.4","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.9.4?os_name=debian&os_version=bullseye"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Nov 2023 18:59:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:ca426296fe928600d0b4b844aee43e2b70a05c6f4032de5f65dcc49f5cedfd82`  
		Last Modified: Tue, 21 Nov 2023 06:31:08 GMT  
		Size: 30.1 MB (30064123 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a7125e296ac071a07e741c080fa505548be787bc563978ba1f28cbadf817a297`  
		Last Modified: Wed, 22 Nov 2023 11:43:36 GMT  
		Size: 2.2 MB (2210605 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:2e49f9e29dfad28718cd108a919638b129d2262ff57b91ffe20461688b811be4`  
		Last Modified: Wed, 22 Nov 2023 11:45:31 GMT  
		Size: 142.7 MB (142731447 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:df3400a0265f902d7d8c9e834d5073fe5df92d990c31a31d8b2c6d2558cb20e3`  
		Last Modified: Wed, 22 Nov 2023 11:45:27 GMT  
		Size: 375.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:bullseye` - unknown; unknown

```console
$ docker pull julia@sha256:fb2d38de8afc145ffbb6332acc6df70e86bc9d2b66b225dad2a6e580798c547d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 MB (2249683 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0ebd96616f57b741f3fed5df6f64e01b74b1d9dbccea3ad773850dafabeb87e3`

```dockerfile
```

-	Layers:
	-	`sha256:46a6cdaf3cb65d639ac13c503e659475f686beefe4c4cc780d3f259614fcbb14`  
		Last Modified: Wed, 22 Nov 2023 11:45:27 GMT  
		Size: 2.2 MB (2231688 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6fc944b0ea52d05826731138ee3e92df094ad55f33d67212e257f7e4720cf87a`  
		Last Modified: Wed, 22 Nov 2023 11:45:27 GMT  
		Size: 18.0 KB (17995 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:bullseye` - linux; 386

```console
$ docker pull julia@sha256:476afe65e0257c3d8658218569e932ebc9e8b4bfd27ea99e10d0c785087471f4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **172.0 MB (172003702 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e76691d648feafe240bb0943f3399f5263240e437f70a066f4a96c08fb795ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 14 Nov 2023 18:59:25 GMT
ADD file:7de881b584405a880c4d02778056aaa81bb5dd5d1af65b3086d66aed9ff0ad4b in / 
# Tue, 14 Nov 2023 18:59:25 GMT
CMD ["bash"]
# Tue, 14 Nov 2023 18:59:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 14 Nov 2023 18:59:25 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_VERSION=1.9.4
# Tue, 14 Nov 2023 18:59:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.4-linux-x86_64.tar.gz'; 			sha256='07d20c4c2518833e2265ca0acee15b355463361aa4efdab858dad826cf94325c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.4-linux-aarch64.tar.gz'; 			sha256='541d0c5a9378f8d2fc384bb8595fc6ffe20d61054629a6e314fb2f8dfe2f2ade'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.4-linux-i686.tar.gz'; 			sha256='2b045a30c6ed8b14a5f4b7ecfb74ef2af7d70b85c9b513cd347886c8dace39bd'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.4-linux-ppc64le.tar.gz'; 			sha256='a5da86c0f0f4ef6d8645f74d8397a6e833831ee212de9edc52e4aefe8f368494'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.9.4","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.9.4?os_name=debian&os_version=bullseye"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Nov 2023 18:59:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:75c11612678b54e79a38118fe66e532c61b3d0798afb741007b4cd3209c0ec4e`  
		Last Modified: Tue, 21 Nov 2023 04:45:24 GMT  
		Size: 32.4 MB (32402632 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:eaf77a7e3dcacc4a1043fa1c037fa9a8583f65494a1246989400af9307fe3293`  
		Last Modified: Tue, 21 Nov 2023 06:16:57 GMT  
		Size: 2.3 MB (2328502 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3a0d4a07e91a710fe9d4d3013c0c262a50839c022b13e58dbfab77790b36a194`  
		Last Modified: Tue, 21 Nov 2023 06:17:01 GMT  
		Size: 137.3 MB (137272199 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:87b75c38a506843d6b9584389c90c812f421bea82cd64356e842e3bfe91dd8c2`  
		Last Modified: Tue, 21 Nov 2023 06:16:57 GMT  
		Size: 369.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:bullseye` - unknown; unknown

```console
$ docker pull julia@sha256:0acf883b7f3680e240988333c96fe70a9ec8952e2285ff9df1b85211a7d91adc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **17.9 KB (17906 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0b6828dcf1a158fb56c58d412c564b98b67462775453b5f1a9ee1234860072b5`

```dockerfile
```

-	Layers:
	-	`sha256:dcb4433b872a24937f3fc728f44e58583a87c48ec8f51d4373621ffceb06c79c`  
		Last Modified: Tue, 21 Nov 2023 06:16:57 GMT  
		Size: 17.9 KB (17906 bytes)  
		MIME: application/vnd.in-toto+json

### `julia:bullseye` - linux; ppc64le

```console
$ docker pull julia@sha256:181b70d9d5ea333f428497ad5149997451ee0c8a96b04846a058e5ed4b39a466
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **170.7 MB (170705442 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb89c03f957007e04b2d273e49fe2e079bd7b89090c407324da09c1b00ee3306`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["julia"]`

```dockerfile
# Tue, 14 Nov 2023 18:59:25 GMT
ADD file:b0d18f2d04821eb50d1faecc1a64916f5c63dd386ae71a3b2cb1d6c4aac6e1c4 in / 
# Tue, 14 Nov 2023 18:59:25 GMT
CMD ["bash"]
# Tue, 14 Nov 2023 18:59:25 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_PATH=/usr/local/julia
# Tue, 14 Nov 2023 18:59:25 GMT
ENV PATH=/usr/local/julia/bin:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_GPG=3673DF529D9049477F76B37566E3C7DC03D6E495
# Tue, 14 Nov 2023 18:59:25 GMT
ENV JULIA_VERSION=1.9.4
# Tue, 14 Nov 2023 18:59:25 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		gnupg 	; 	rm -rf /var/lib/apt/lists/*; 		arch="$(dpkg --print-architecture)"; 	case "$arch" in 		'amd64') 			url='https://julialang-s3.julialang.org/bin/linux/x64/1.9/julia-1.9.4-linux-x86_64.tar.gz'; 			sha256='07d20c4c2518833e2265ca0acee15b355463361aa4efdab858dad826cf94325c'; 			;; 		'arm64') 			url='https://julialang-s3.julialang.org/bin/linux/aarch64/1.9/julia-1.9.4-linux-aarch64.tar.gz'; 			sha256='541d0c5a9378f8d2fc384bb8595fc6ffe20d61054629a6e314fb2f8dfe2f2ade'; 			;; 		'i386') 			url='https://julialang-s3.julialang.org/bin/linux/x86/1.9/julia-1.9.4-linux-i686.tar.gz'; 			sha256='2b045a30c6ed8b14a5f4b7ecfb74ef2af7d70b85c9b513cd347886c8dace39bd'; 			;; 		'ppc64el') 			url='https://julialang-s3.julialang.org/bin/linux/ppc64le/1.9/julia-1.9.4-linux-ppc64le.tar.gz'; 			sha256='a5da86c0f0f4ef6d8645f74d8397a6e833831ee212de9edc52e4aefe8f368494'; 			;; 		*) 			echo >&2 "error: current architecture ($arch) does not have a corresponding Julia binary release"; 			exit 1; 			;; 	esac; 		curl -fL -o julia.tar.gz.asc "$url.asc"; 	curl -fL -o julia.tar.gz "$url"; 		echo "$sha256 *julia.tar.gz" | sha256sum --strict --check -; 		export GNUPGHOME="$(mktemp -d)"; 	gpg --batch --keyserver keyserver.ubuntu.com --recv-keys "$JULIA_GPG"; 	gpg --batch --verify julia.tar.gz.asc julia.tar.gz; 	gpgconf --kill all; 	rm -rf "$GNUPGHOME" julia.tar.gz.asc; 		mkdir "$JULIA_PATH"; 	tar -xzf julia.tar.gz -C "$JULIA_PATH" --strip-components 1; 	rm julia.tar.gz; 		apt-mark auto '.*' > /dev/null; 	[ -z "$savedAptMark" ] || apt-mark manual $savedAptMark; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		julia --version; 		echo '{"spdxVersion":"SPDX-2.3","SPDXID":"SPDXRef-DOCUMENT","name":"julia-sbom","packages":[{"name":"julia","versionInfo":"1.9.4","SPDXID":"SPDXRef-Package--julia","externalRefs":[{"referenceCategory":"PACKAGE-MANAGER","referenceType":"purl","referenceLocator":"pkg:generic/julia@1.9.4?os_name=debian&os_version=bullseye"}],"licenseDeclared":"MIT"}]}' > $JULIA_PATH/julia.spdx.json; # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Tue, 14 Nov 2023 18:59:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 14 Nov 2023 18:59:25 GMT
CMD ["julia"]
```

-	Layers:
	-	`sha256:60239a74847cd7e9a928353188f3cf096ca8cf648e2b27c765058e169d568fd9`  
		Last Modified: Tue, 21 Nov 2023 04:29:47 GMT  
		Size: 35.3 MB (35293727 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:06d0b56875b7f6abcabf7daf112d7d3cae85e898980949b37dab187bcd05a907`  
		Last Modified: Tue, 21 Nov 2023 20:45:05 GMT  
		Size: 2.4 MB (2424863 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a8377da2ff2ce841b8692ccdf43f2b3fa23bc5aea91ad746dc760328163757cc`  
		Last Modified: Tue, 21 Nov 2023 20:45:08 GMT  
		Size: 133.0 MB (132986476 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39256c7032644d483bea628350891591db67de985379d379edfa4ab15fd29997`  
		Last Modified: Tue, 21 Nov 2023 20:45:05 GMT  
		Size: 376.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `julia:bullseye` - unknown; unknown

```console
$ docker pull julia@sha256:275619bc38e638077a9c98d99214a638f8b6f2d86e1d95adfbab5a25f5de8f81
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.3 MB (2254058 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3d8ceb1070ec4b553fc63661dfc150785bb6e95330a6f96f3ebee069600046b7`

```dockerfile
```

-	Layers:
	-	`sha256:b27363162e86a4b4613a2eabe4d13d8266fc9e628dedd016ef62e278df16461b`  
		Last Modified: Tue, 21 Nov 2023 20:45:05 GMT  
		Size: 2.2 MB (2235866 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:36fed235c14ed6dd250e4f6debaf78754b6863b22b25a32ed309c39e9ad87667`  
		Last Modified: Tue, 21 Nov 2023 20:45:05 GMT  
		Size: 18.2 KB (18192 bytes)  
		MIME: application/vnd.in-toto+json
