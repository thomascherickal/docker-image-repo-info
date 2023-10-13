## `memcached:bookworm`

```console
$ docker pull memcached@sha256:ed865c1d2b5a6ca7337e5ded3e64be89d950080340831ef3a5b7cece005cac42
```

-	Manifest MIME: `application/vnd.oci.image.index.v1+json`
-	Platforms: 14
	-	linux; amd64
	-	unknown; unknown
	-	linux; arm variant v5
	-	unknown; unknown
	-	linux; arm64 variant v8
	-	unknown; unknown
	-	linux; 386
	-	unknown; unknown
	-	linux; mips64le
	-	unknown; unknown
	-	linux; ppc64le
	-	unknown; unknown
	-	linux; s390x
	-	unknown; unknown

### `memcached:bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:8af51889f0f774a00f36624e58faac309c258eafb8054c6abc6fbbb56c78d0a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.8 MB (38811465 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0fa23f6ace109fad9223ea2db53f79afa8b91b14051c61305f82bc2c781a788c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:55ad846fa191e603f48090eae0e4a7149c4066b94406593ec1898ad2c3347937 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:a378f10b321842c3042cdeff4f6997f34f4cb21f2eff27704b7f6193ab7b5fea`  
		Last Modified: Wed, 11 Oct 2023 18:39:34 GMT  
		Size: 29.1 MB (29149874 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e68aaf702a54364b3f216204ad2725f5b416fe496294086899b821bb5133552d`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0fb853802e1447e9b1dbe3e8a86f27a5691286127397adf8d52f943d16b80042`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.5 MB (2488274 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fcc9694d882f053fcf2e7bb33709dcb86eef6c29c3187c190ad93852af7a50f2`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 7.2 MB (7171802 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fde136907f7040bd6126a5b2c0bca844fef33e2fc804c1f135e99393869cce4c`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c121d0db5ccb2988b1fc0c76ce60a2e78309d77b264adf99e815e1ecf2c6a957`  
		Last Modified: Wed, 11 Oct 2023 20:07:28 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:888d3aaaddc944acb247f0e42586c8c8a7f8c3262166ee89ceda0dbe3998cafa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2911211 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:06530a2f7a54ba7d86fc6cee0da9a46ea1aea89dc4beecbee6d54ed8eee82dd9`

```dockerfile
```

-	Layers:
	-	`sha256:7bbbdfb4ba86ed51b46d2fb83bf8cf4e095da6d5c9dd89697a3488dd392414d7`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 2.9 MB (2889442 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:6fe7a995830937695f7110928df7e791673ab04015add73a1f2e9ec661bbc60f`  
		Last Modified: Wed, 11 Oct 2023 20:07:27 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:a6919fc9976aa2c291f194860f40fcc9499d33cbd2592af9087e5d64b7930602
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **34.8 MB (34846023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d5222dddac963b84d55ef902d40fa3f949ee73caac9614ca77c1f4a81ef009c6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:8c43adb3245fc6f2b10aa5a86c850db5dcf3515eaf7e46630922fe21f806bd2a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:904e6393ef1ee28b37171369eb4f7cb04714631c711799819fccb83886bd212b`  
		Last Modified: Wed, 11 Oct 2023 17:40:47 GMT  
		Size: 26.9 MB (26922150 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f0569355cb85b70d6a614ea9604289ce8e724f0f9ff4d1d8a12afc24c4c9ad1f`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6939032c8ff0687b012a85d3411c702266b934a677f96eb521658b44f5b4a8c0`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 2.1 MB (2089182 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:8e8a2a7338b5cacc7b6e4e3db2359eebb1936b0b14266d5bad0dfcc21c9becff`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 5.8 MB (5833176 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19f35a8116fe7e124bee612b2ac511694077a1f35f76ed056903987ab4921e34`  
		Last Modified: Thu, 12 Oct 2023 08:32:06 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a43775be6dfac6c255e35b164eacd7328df241f33f9245206a8eaf481062ccbc`  
		Last Modified: Thu, 12 Oct 2023 08:32:07 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:f1276a05a4db6e8b7bb9d8374d480b85a79f1b92d4e7475c65e247bf1427200c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fe67b683a818ed7c22a49086ec4f22e53c6efa9040becea46adb07f550dae564`

```dockerfile
```

-	Layers:
	-	`sha256:12ecc330d2059d33dc7a7c518e7be06804f5fcadafdc8e2db030631f5c92b326`  
		Last Modified: Thu, 12 Oct 2023 08:32:05 GMT  
		Size: 21.7 KB (21695 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:bec9ef3ee60f5e451d39922e498dd2f27711970644c2ccd55b6c6eaa4580f93c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.7 MB (37708978 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e517aeb64383b97eb41d514faca037212d3c6c9ae5dc95721d55937f40c106ec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:5c81bfc00a28feb4079c0daa743f829a6a5bbc1a9d40a890cb49e420539a7f15 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1bc163a14ea6a886d1d0f9a9be878b1ffd08a9311e15861137ccd85bb87190f9`  
		Last Modified: Wed, 11 Oct 2023 18:28:28 GMT  
		Size: 29.2 MB (29179284 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:28c06e06713bb0febebb47594bef8ec8f6cb3e3eca681c38d02fa42f1e7b6e65`  
		Last Modified: Thu, 12 Oct 2023 20:55:20 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d2d9d520f69da9326b976055fb082032c7cdbad455528b2539961dd229653c8`  
		Last Modified: Thu, 12 Oct 2023 20:55:20 GMT  
		Size: 2.3 MB (2346655 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3113d25e3f88e67f6c2698ca7be64fb9dcd083e25beaa25afd80006bbae7c60c`  
		Last Modified: Thu, 12 Oct 2023 20:55:21 GMT  
		Size: 6.2 MB (6181522 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:39e84526ee25ed86c0aed93088c7b7990894bf8909ecc7fb8d4cc82405a0d13b`  
		Last Modified: Thu, 12 Oct 2023 20:55:20 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4ecc74ed169e6d51ed06db21f33bf28e54ecf3415eb6dabd8134dc26f69f844e`  
		Last Modified: Thu, 12 Oct 2023 20:55:21 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:8f2b58a673fb76a59d7bd46a915d1b78247c76d2f3505659d721d894ead18ace
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2892605 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b021ba5041f1b73c5f7dbb5244e246a33a70a056f65e596cfbaf3ab3e34dd8aa`

```dockerfile
```

-	Layers:
	-	`sha256:c1da26f25c772b02e84de5f64d4090493a8bf574cee4c9395a2796926f04339f`  
		Last Modified: Thu, 12 Oct 2023 20:55:20 GMT  
		Size: 2.9 MB (2870985 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:9970e9db8a77902c18609737cd357696ed77b0d2a0f8a4fb9fbebc50a3cf3ffd`  
		Last Modified: Thu, 12 Oct 2023 20:55:20 GMT  
		Size: 21.6 KB (21620 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; 386

```console
$ docker pull memcached@sha256:2a0280d1a33338b5a3131ef0d177a55f64b257eae2f8926dfa1ac7f621a4b8c7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39291816 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d264cd3e267b6de821fe419bf562c44c968ef77f5cac4521ffd355d9f41c73e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:31318c1b1f05d559cce42f5b12eef97d916932217e0b987fb07c0fc11bf0a14a in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:b27d0f1369837277a82877763487cdd2535037988fc27e16f11cf74e103ae4cd`  
		Last Modified: Wed, 11 Oct 2023 17:45:31 GMT  
		Size: 30.2 MB (30164118 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1c6330eea924269383a3b7e9131800150c66c31569d0b88e8f37ebf658d6da3e`  
		Last Modified: Wed, 11 Oct 2023 19:04:40 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:a0fa225eb005c61654844b15f00777bb4f3e4b0bfada4e8a1756f11eec7b59fd`  
		Last Modified: Wed, 11 Oct 2023 19:04:40 GMT  
		Size: 2.5 MB (2492374 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:99beba03bc71c45e596c1d57fd6af21307ea9bb62950e58bca00eed4a974b729`  
		Last Modified: Wed, 11 Oct 2023 19:04:40 GMT  
		Size: 6.6 MB (6633812 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4abd1977fee3070e09d9c73d2e2ed9a0a651ee1bb0fc43b81088cca8f2281bb0`  
		Last Modified: Wed, 11 Oct 2023 19:04:40 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:64d2d01857fc1db2dd51a731bf176fe1a91bda68373bc5476e6188f39910d417`  
		Last Modified: Wed, 11 Oct 2023 19:04:41 GMT  
		Size: 120.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:c5eed6e91c162ebb297578e39303eb70fb727f6828fc155ee6d05e8daf111cc8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8413dc2139f71a819d1aa989e76801abcd9af351beefd69d9af34d01bc48e2d`

```dockerfile
```

-	Layers:
	-	`sha256:7096fdc893f3ed1ec425e26ecf864a1f2c5ef5b908c77a7f418c690089835542`  
		Last Modified: Wed, 11 Oct 2023 19:04:40 GMT  
		Size: 21.5 KB (21499 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:575825bdbf62fc255547394ef491710ba88f0be3ca735eaf246ece06f13363ef
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.4 MB (43398233 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3f951153522f4d9719c37a9862412f3e29e487d11322c5ff7a009cf8becca1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:850547a08e38ebc5a3659df86e70039a8d9828ae26ae485b077c98a959248dcb in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:0f581c6294fe7421dfee024e2c7dddd73ef3fbd7ff23b05bc3c1bf9f50885e85`  
		Last Modified: Wed, 20 Sep 2023 03:20:59 GMT  
		Size: 29.1 MB (29121674 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:15e25af5488ea4ad0df132fa2c22a282c1a17ad1460cdb25fe5939e03a753528`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 1.1 KB (1113 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:19a5f416c9bf283212262e33fe8529d0ff3917fcee1e8ca9fb058170fd528211`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 1.9 MB (1934931 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:05862af95003d85f9a1b5696dfb3588bdd8e34c74f067d845b722d70edfc679f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 12.3 MB (12340111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:e8aae13855c46b73d2506b2d91036f6f0b4bc63b7d7ec12ecc63fd672c64c0f7`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0709f88ce6a011ea45fd41c091ee6fcf4baa0610e0591a9fe0d10626eaf9475f`  
		Last Modified: Tue, 03 Oct 2023 19:04:41 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:269b3e28059bf711ac45886388e91fa405b8a1e0ca1a114acefc997bbdad6d05
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21491 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1059a2662b538952006866f53463fcea773b5e090eaead3a4ad49f4d0a656ae5`

```dockerfile
```

-	Layers:
	-	`sha256:e1052b07541ae6e041e59834c527075b62df62a33f7a9b9e96fda4b6237e83df`  
		Last Modified: Tue, 03 Oct 2023 19:04:40 GMT  
		Size: 21.5 KB (21491 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:a7a294c969fdfafa2ee6fdc20aa85f0b2561beb3eb5351349145cd3c7ad77b47
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43027015 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c0f918da1241c3a49506ba77c6fc96d8fdfffc3a8e4e128db5b2950a04fa1560`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:53c83bdd58e7c4003ae769596cc2f8e6b72c0bbb854dbe7f006a39f273848b1b in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:54813908ce8a5d8a81f2db88ad0366eb5266484c7c402e5e93ef26e764f7a0e2`  
		Last Modified: Wed, 11 Oct 2023 17:49:58 GMT  
		Size: 33.1 MB (33141653 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:da17b0744296ecb848ef17404c2d1226eec6572fc961c0e4b5c81c2fbfd61651`  
		Last Modified: Thu, 12 Oct 2023 18:48:27 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b29b164adc7432dfef9a43d2a0cd60f32f846a054313fac84ebd4790ce13746a`  
		Last Modified: Thu, 12 Oct 2023 18:48:28 GMT  
		Size: 2.7 MB (2697819 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:3e127db4854edf691f2ae5b795dece62f7f0e57e71e38f8de36d66de9b9828e2`  
		Last Modified: Thu, 12 Oct 2023 18:48:28 GMT  
		Size: 7.2 MB (7186026 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c87d512f51c2bc47fb3d279a76dc5313cd73a2d5b20f0acf9659634f7fa8c9a1`  
		Last Modified: Thu, 12 Oct 2023 18:48:28 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:716c7c2c815875417e431b4c261211a4a5e9806bc32ef7376b6fbdcf47a05ffa`  
		Last Modified: Thu, 12 Oct 2023 18:48:29 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:29e92260bcda635b16520f963c4cce7cbf1ef83a14fcdc92ce647c22720746ae
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2916853 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:02ae378fe4c43d5a7be1d39282cacdef03550d9038bd8e5f29cb178e68a0e03d`

```dockerfile
```

-	Layers:
	-	`sha256:804f75078a895e58ef49702a83631b735601c6602c12b275bf8e435d812e4b27`  
		Last Modified: Thu, 12 Oct 2023 18:48:28 GMT  
		Size: 2.9 MB (2895016 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:1c9d2c22fdf21ab7c82333bd989f1cdd164d1c8f3372315a49451692cec03cbc`  
		Last Modified: Thu, 12 Oct 2023 18:48:27 GMT  
		Size: 21.8 KB (21837 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:69e715ddcec33599de691ec6d15310210be993097b2a8e48eaf1290c729099a2
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **35.7 MB (35741721 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f74303d426c9d90f80c849de21bfaa1f7be233741561c120592b0f7897f1371b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Fri, 16 Jun 2023 06:54:11 GMT
ADD file:b85ed0ed01200dd3626d66cf5205d989fc48e61b3dd3498f777ee72d91e64870 in / 
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["bash"]
# Fri, 16 Jun 2023 06:54:11 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_VERSION=1.6.21
# Fri, 16 Jun 2023 06:54:11 GMT
ENV MEMCACHED_SHA1=6d899680b4ba4b76b6c92120143cf87630ee984a
# Fri, 16 Jun 2023 06:54:11 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Fri, 16 Jun 2023 06:54:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 16 Jun 2023 06:54:11 GMT
USER memcache
# Fri, 16 Jun 2023 06:54:11 GMT
EXPOSE map[11211/tcp:{}]
# Fri, 16 Jun 2023 06:54:11 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f270c1bb05fa46b165ce3680225dc9fa5bbfe4d69420a467350e80f692c78eb2`  
		Last Modified: Wed, 11 Oct 2023 17:56:03 GMT  
		Size: 27.5 MB (27512850 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ae1893bbcc0e0a27ce1282dfb1b2d5a8e546bf79eb505d551105b373ea20c280`  
		Last Modified: Thu, 12 Oct 2023 12:45:12 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:f3fde33c31632ef2c747018b1f30b030522f5cbdd84b1c2784503b0c4659d618`  
		Last Modified: Thu, 12 Oct 2023 12:45:12 GMT  
		Size: 2.2 MB (2152430 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:321d9e1625addb79dc12d32ef3e4d08d32402454af4a5062480c82b10169873c`  
		Last Modified: Thu, 12 Oct 2023 12:45:13 GMT  
		Size: 6.1 MB (6074925 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c4412f9686bcab10b27d7b9708236759b1c5a5483f0c15c40dbef126b8e19fc7`  
		Last Modified: Thu, 12 Oct 2023 12:45:13 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b36dda7eee6b46834f68d06ec9e6364226552daded5b5ba8c5ba31272e5c5f6e`  
		Last Modified: Thu, 12 Oct 2023 12:45:13 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:934ca96150284b8aa8cfe069e475822208d5426c398fa448a86c27450ce29e62
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 MB (2899064 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed8fbcc42bc581e580e3fab02f639fcbf3636d893fb41366db489f0f8aacfa34`

```dockerfile
```

-	Layers:
	-	`sha256:0d440f321339ab1a2ee4f875bd6fb3600f61be824158efb8213df7e582464800`  
		Last Modified: Thu, 12 Oct 2023 12:45:12 GMT  
		Size: 2.9 MB (2877295 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:d74bfb3fd827ae114580e8fd86cdb3addf116515f141393e42fb31cb3925a84b`  
		Last Modified: Thu, 12 Oct 2023 12:45:12 GMT  
		Size: 21.8 KB (21769 bytes)  
		MIME: application/vnd.in-toto+json
