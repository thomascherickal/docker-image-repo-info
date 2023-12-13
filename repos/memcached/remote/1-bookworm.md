## `memcached:1-bookworm`

```console
$ docker pull memcached@sha256:4532a2216636686fbd21b1d768684ea5efd37103163c323a9073eb32eff2cb9a
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

### `memcached:1-bookworm` - linux; amd64

```console
$ docker pull memcached@sha256:0d358fa0198562aa3d1e1c3e9386e1835256875517d8a4786f3dd50a1f65f1de
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **41.1 MB (41125606 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:03bad2c21b5df5c82f8c581ebec403482a3e00c0f35697ca669c46a7d000a13d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:21:37 GMT
ADD file:d261a6f6921593f1e0b3f472ab1b1822e2c6deb0b369200f0b3370556bfad017 in / 
# Tue, 21 Nov 2023 05:21:37 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:1f7ce2fa46ab3942feabee654933948821303a5a821789dddab2d8c3df59e227`  
		Last Modified: Tue, 21 Nov 2023 05:25:58 GMT  
		Size: 29.1 MB (29149908 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:21ac6fd160890cbc46a76542eb3f68654f3e3fb043b1b28a18155ec6863d60bc`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:6330fc82e1304befcc27a7598cd1a85152985d06426f94966788bf5a1583dcc6`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 2.5 MB (2488284 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4047c827380f04698fbc51155441d719f93b84c1a092d633260c704f286296dd`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 9.5 MB (9485895 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:401b5de2a4f8d9f588888754fa8347b67590c776363770f46ef67688116a4a0c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:ee899f9aed95096580ea4a2325fd4824518ff1621f433f393fa253b52b7294b5`  
		Last Modified: Tue, 12 Dec 2023 20:52:58 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:5ccb88c1a86bd6524b6d5c9383254cdd79314d656a0c982658ecd35d9716431b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3077929 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:238ef9023561adc9c09faf875c5370cb2711a83cc7327dcc49ae7f8255c23794`

```dockerfile
```

-	Layers:
	-	`sha256:f84a6f3d0bdab8613be68ff091a6a78bedf8f697d4df55ff90ac7b745337e72c`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 3.1 MB (3056812 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:8d7aee053ab87a86e42ba3d14810d3f1918c6e66d4d3ef02bc9c741f3948b83e`  
		Last Modified: Tue, 12 Dec 2023 20:52:57 GMT  
		Size: 21.1 KB (21117 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; arm variant v5

```console
$ docker pull memcached@sha256:cb9426984b18b2d3df1c5fbb2bb7e2e9ebe08325d4adce6d0cd7a9207c413476
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.1 MB (37113170 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0a8f2fb6119b629983f190d8b73208a156991d8cb65c47579a68125c339e9c75`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:00:51 GMT
ADD file:1ae8e5ac45b11d01083680b765e1fcfef9f7938f89d6f424572126fa946d8cdf in / 
# Tue, 21 Nov 2023 05:00:52 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:f476aef5b6e1122850e68c81ef06fc2df17e968961b060483b4d2fb33018aae3`  
		Last Modified: Tue, 21 Nov 2023 05:03:55 GMT  
		Size: 26.9 MB (26922153 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:89367ca16d2c3104d44514e1b9b94b0ac4070ea0f6f04523c72dda62795f3a17`  
		Last Modified: Tue, 12 Dec 2023 21:47:13 GMT  
		Size: 1.1 KB (1110 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5ecbc6577cf78c09bd4136f78a57a904ae1ab705fce8595e8d1187d800158e6f`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 2.1 MB (2089289 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:12f8a270079b04e1372c73cc16ff2ae33e6f6ee0dcc7e8ed57843fca20b3d038`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 8.1 MB (8100211 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5f592556023f9ba6125ecf6b89156ba61c05526ad324708c3d2a09600ee5e7e4`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:fa757a09f6a7a23114a13869f15b229384628cf108567d395dc0d4730c685409`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:0c93e2660a508733f1c7d5236af77ef81fbcd0b27e4ac55c81d83334c8794891
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.0 KB (21043 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538fbf714aa2f8a4175400dd43b0715e416f73fe598fc50d3f763afa144595da`

```dockerfile
```

-	Layers:
	-	`sha256:f65b3a9a0f6936cae3c1e411ecdd846d754a1978d851fdacf4b25526cb9ff4cc`  
		Last Modified: Tue, 12 Dec 2023 21:47:14 GMT  
		Size: 21.0 KB (21043 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; arm64 variant v8

```console
$ docker pull memcached@sha256:c5adc5a4207d95c96a36131c2d39085b082f0e22f4595b935e72bcb463c10383
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **40.0 MB (39979924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:cf26c17403ed5a4db96ddd8b41aeb2fd45483f897882a57972c994c95a44c5dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 06:27:06 GMT
ADD file:869c7d0747a17c53715581a2e862992eb8516c7f45f167821dfa80966a4870d1 in / 
# Tue, 21 Nov 2023 06:27:06 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:2c6d21737d8318aa15c4cc838475029a5efc36c0429e3d8da80d97d0b96d9aaf`  
		Last Modified: Tue, 21 Nov 2023 06:30:30 GMT  
		Size: 29.2 MB (29179277 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1a39d6fec0d552a8078ab223bafd58bc9a0c8c27c26600a5b95c6a521bb97f3d`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d1ceea69964553dd3aaf853e0d7b753495cab4623b9377c69096be0bdf88146`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 2.3 MB (2345975 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:52063b8e37cbc1e5e6e3af0f54b834ae3f6a53d023349ae819c9607e5fc98aec`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 8.5 MB (8453155 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5b99d0095a64f8110efee1f5e91754cc923294d50c9e2927e515354746a3f465`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:913c9e21eaa9c49c99b1b39e5cda0ef12356220075c869ea4776dca36fe83b75`  
		Last Modified: Tue, 12 Dec 2023 23:43:18 GMT  
		Size: 121.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:3d519a2eb9e00b43e6bc7584f6962b12ba032c4487a6e4ef7fd2b00b667bc90d
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3053138 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9cc25288d58197dcc1309ea4a8128d0b120b92ad2d877f226095cd4847696474`

```dockerfile
```

-	Layers:
	-	`sha256:c5edc5ba98b4e6a438caa0d4541784c5c1e8b23d6020bc0b2a5b9910d0725400`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 3.0 MB (3032003 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:b15e35765293b6f1da0e628c94108f229423c5a6379b8b5c47a41415f377b6d8`  
		Last Modified: Tue, 12 Dec 2023 23:43:17 GMT  
		Size: 21.1 KB (21135 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; 386

```console
$ docker pull memcached@sha256:fa9dba8086765d68f2feecfc2ac08fb29c019597d09943bb480227e6cba87666
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **39.3 MB (39294993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93047050e75b6d4d64adb8a7c8f68cb118bad27ca9dc772120e251b174752cf9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:0c94521fdd9c0a4fdeeb9aad23e68cd053fba0dcd7c3af550aefa79377816e31 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:98bdfce9af831c2a0d0bfcca812d0039cd1666986550f552b4b4c625bd5aa31c`  
		Last Modified: Wed, 01 Nov 2023 00:43:26 GMT  
		Size: 30.2 MB (30164042 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:1b647d4b10cf20ac5807101c7d0380701be684aa82f5c01ec41f674b5ef23d42`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 1.1 KB (1109 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b61c058003459de4911c2901b2d799b03de754a1b9e64ffbe21a04992e962e62`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 2.5 MB (2492501 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:810b6db64df2fcc8f76941cdac75093cf35bd72ac3cd1fa5eb664e74c1f67cd8`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 6.6 MB (6636937 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:dbb899942df4149bd5fae8bac6e295285ec80f82d621f2b29c931ee348491cfb`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 282.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4a8530160ab232c37c0ddcbf5e3a731d835d378d1382843957f6c2a73b2b5be6`  
		Last Modified: Wed, 01 Nov 2023 01:06:50 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:dd7ce9519c31365127142232df2ed0b285e9acc03cd77c23c838bf932165def8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.5 KB (21498 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eef82c92e07c11a92c337806d01cfb1c6cdc7a16608dcf304a38de34d2ef1dbb`

```dockerfile
```

-	Layers:
	-	`sha256:c0d9dd22513f8d3e791e1796d7ef1906e57c798c92dd35d0be9cf2eaecec5954`  
		Last Modified: Wed, 01 Nov 2023 01:06:49 GMT  
		Size: 21.5 KB (21498 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; mips64le

```console
$ docker pull memcached@sha256:a7c198db1b0856aff4b1514137e473ea30bce2ef22f0192cfdce7e2e44f2a863
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **37.6 MB (37588022 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1654ec4454e597d7e7cb6a7d97e98208de241a3dfafc5e0532b9561eac91f013`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:e093749192323dc72b60a8440ddba26c415586f618b5e107fa264ba5eb2ca7ba in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:ebdff2138fee4a3ec27560ab1353dc51c12c2608ff721f5db3d24104872b702a`  
		Last Modified: Tue, 21 Nov 2023 04:20:35 GMT  
		Size: 29.1 MB (29141984 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:50b1ffce24cec457fe1757715d60bd669145e5babade7c57143c4b665a55389e`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 1.1 KB (1112 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:893c712c491a058aada36756e9f176b6c6c2f3a2b3adf0cd94b896c8198ec3ee`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 1.9 MB (1937483 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0b8443254952572331df084976853329b69a4348b3c620bb073b5c89fb943b2b`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 6.5 MB (6507036 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:904bfc5c5c0923edd9be421332402b224bfcd49053bc9b3fae6173383f5cd395`  
		Last Modified: Thu, 23 Nov 2023 01:10:59 GMT  
		Size: 285.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:c265216ad3407dbc99903d96423b3a2314bc48cc0118911d150a6bb087ff7d85`  
		Last Modified: Thu, 23 Nov 2023 01:11:00 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:e2fcd32899d09ff06793849927220bea14475e64f085972afbc1f3af74dc209b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **21.7 KB (21656 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bf1c2028769aa20a3e529d0f85c8144ba6b099f74cda0dfca2272b7831d2d7a5`

```dockerfile
```

-	Layers:
	-	`sha256:75bab713cb94cdececf4c3879050737e7cb4bbb6206daa071ea001692b53d659`  
		Last Modified: Thu, 23 Nov 2023 01:10:58 GMT  
		Size: 21.7 KB (21656 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; ppc64le

```console
$ docker pull memcached@sha256:d8d106a88d6a15fadf738e59a6dcfc3942f11c7a2d19b7473abce66af7f4d19c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.0 MB (43030916 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:85da4ca798d44fc951b843ec85c410207ecc3c56af6d1bf7c321c91266d54e1b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Mon, 16 Oct 2023 06:54:12 GMT
ADD file:8b22a531b6611a1e63dfc20e4e2931592e2d821bd4b64c4b2810bb9a36640c02 in / 
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["bash"]
# Mon, 16 Oct 2023 06:54:12 GMT
RUN groupadd --system --gid 11211 memcache && useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 16 Oct 2023 06:54:12 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 16 Oct 2023 06:54:12 GMT
RUN set -x 		&& savedAptMark="$(apt-mark showmanual)" 	&& apt-get update 	&& apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	&& rm -rf /var/lib/apt/lists/* 		&& wget -O memcached.tar.gz "https://memcached.org/files/memcached-$MEMCACHED_VERSION.tar.gz" 	&& echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c - 	&& mkdir -p /usr/src/memcached 	&& tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1 	&& rm memcached.tar.gz 		&& cd /usr/src/memcached 		&& gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)" 	&& enableExtstore="$( 		case "$gnuArch" in 			s390x-*) ;; 			*) echo '--enable-extstore' ;; 		esac 	)" 	&& ./configure 		--build="$gnuArch" 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 		$enableExtstore 	&& nproc="$(nproc)" 	&& make -j "$nproc" 		&& sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf 	&& make test PARALLEL="$nproc" 	&& mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf 		&& make install 		&& cd / && rm -rf /usr/src/memcached 		&& apt-mark auto '.*' > /dev/null 	&& apt-mark manual $savedAptMark > /dev/null 	&& find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	&& apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false 		&& memcached -V # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 16 Oct 2023 06:54:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 16 Oct 2023 06:54:12 GMT
USER memcache
# Mon, 16 Oct 2023 06:54:12 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 16 Oct 2023 06:54:12 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:c570d04e61d8e35a3c8f12179d048d701451f97f9cf2099ea3e3738512dbf062`  
		Last Modified: Tue, 21 Nov 2023 04:28:58 GMT  
		Size: 33.1 MB (33141607 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:bcd0cf90a66e23cd3d72b99e7d36129b0e846407a07c30031b0c1e4ba115cd30`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:5e4166a0e033df4117b469f840c6f5527e87dbd13c582c0b50c182b4bb3ead79`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 2.7 MB (2698215 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:947b7328e0db59b9870fe9c6d6b7fc4e8a8f1fef3d2a36064fe3d60f5314652d`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 7.2 MB (7189577 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:4f011f72796530a711f1de9d543435299d02ed3636e4cd28aee1fa493fbc2bf4`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9d27046f19e474530b87e1d0b429e9d85f403210dd3d91bf60d8303fef03af96`  
		Last Modified: Tue, 21 Nov 2023 23:46:48 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:4269af6aa39a29d6dca352659fbf04b7d1bb4e65151e63a3ffcf2749d853597e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a6e9626f30d490d2014e9fbb19add0b6ac0f63c8f4af2082d04750fea7ec35ff`

```dockerfile
```

-	Layers:
	-	`sha256:70759e1722d82b89de5c0d71ba2050ecc9f29d95ee758369044a1fc79026a546`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 3.0 MB (3045366 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:4f34d59241ff06b2bd0cb8239d96be938e1e13470264898863f307f84ab275b6`  
		Last Modified: Tue, 21 Nov 2023 23:46:47 GMT  
		Size: 21.7 KB (21670 bytes)  
		MIME: application/vnd.in-toto+json

### `memcached:1-bookworm` - linux; s390x

```console
$ docker pull memcached@sha256:05084fffc798db32442e2cde93eac5815ffd909e9bf65692ac08c9b5ab79e677
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **38.0 MB (38041790 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eac80baab625f3daf940cdb3053e2e709bd61d78d7eae50b7db4d71f87bcd149`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["memcached"]`

```dockerfile
# Tue, 21 Nov 2023 05:04:35 GMT
ADD file:c33fa9fdde73983850798b6eb1cd062e0398109d1d773e6a937fead7475c8efc in / 
# Tue, 21 Nov 2023 05:04:41 GMT
CMD ["bash"]
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	groupadd --system --gid 11211 memcache; 	useradd --system --gid memcache --uid 11211 memcache # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		libsasl2-modules 	; 	rm -rf /var/lib/apt/lists/* # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_VERSION=1.6.22
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_URL=https://memcached.org/files/memcached-1.6.22.tar.gz
# Mon, 04 Dec 2023 18:08:47 GMT
ENV MEMCACHED_SHA1=7a691f390d59616dbebfc9e2e4942d499c39a338
# Mon, 04 Dec 2023 18:08:47 GMT
RUN set -eux; 		savedAptMark="$(apt-mark showmanual)"; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		dpkg-dev 		gcc 		libc6-dev 		libevent-dev 		libio-socket-ssl-perl 		libsasl2-dev 		libssl-dev 		make 		perl 		wget 	; 	rm -rf /var/lib/apt/lists/*; 		wget -O memcached.tar.gz "$MEMCACHED_URL"; 	echo "$MEMCACHED_SHA1  memcached.tar.gz" | sha1sum -c -; 	mkdir -p /usr/src/memcached; 	tar -xzf memcached.tar.gz -C /usr/src/memcached --strip-components=1; 	rm memcached.tar.gz; 		cd /usr/src/memcached; 		gnuArch="$(dpkg-architecture --query DEB_BUILD_GNU_TYPE)"; 	./configure 		--build="$gnuArch" 		--enable-extstore 		--enable-sasl 		--enable-sasl-pwdb 		--enable-tls 	; 	nproc="$(nproc)"; 	make -j "$nproc"; 		sed -i.bak 's/SECLEVEL=2/SECLEVEL=1/g' /etc/ssl/openssl.cnf; 	make test PARALLEL="$nproc"; 	mv /etc/ssl/openssl.cnf.bak /etc/ssl/openssl.cnf; 		make install; 		cd /; 	rm -rf /usr/src/memcached; 		apt-mark auto '.*' > /dev/null; 	apt-mark manual $savedAptMark > /dev/null; 	find /usr/local -type f -executable -exec ldd '{}' ';' 		| awk '/=>/ { so = $(NF-1); if (index(so, "/usr/local/") == 1) { next }; gsub("^/(usr/)?", "", so); print so }' 		| sort -u 		| xargs -r dpkg-query --search 		| cut -d: -f1 		| sort -u 		| xargs -r apt-mark manual 	; 	apt-get purge -y --auto-remove -o APT::AutoRemove::RecommendsImportant=false; 		memcached -V # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
COPY docker-entrypoint.sh /usr/local/bin/ # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
RUN ln -s usr/local/bin/docker-entrypoint.sh /entrypoint.sh # backwards compat # buildkit
# Mon, 04 Dec 2023 18:08:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 04 Dec 2023 18:08:47 GMT
USER memcache
# Mon, 04 Dec 2023 18:08:47 GMT
EXPOSE map[11211/tcp:{}]
# Mon, 04 Dec 2023 18:08:47 GMT
CMD ["memcached"]
```

-	Layers:
	-	`sha256:6daa625e5a040476e253e7acd0befa74254a4865ec836d6334a544d82a21d4be`  
		Last Modified: Tue, 21 Nov 2023 05:10:21 GMT  
		Size: 27.5 MB (27512885 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b19a3143cbec7ddc9a646dbbe779b0b5ec67662cf70e280db146f6ace54ccd61`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 1.1 KB (1111 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:b8af028b1fa76aa55f540dd5be5eaf89eea3fec23e09e9a88550aac36e9ee843`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 2.2 MB (2152508 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:9a774943469875a0902c53fccdd95cad9c18234b759bcdcc5816bd563deb7f14`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 8.4 MB (8374880 bytes)  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:266b4bf499a815da6f7ddcf68e1e61f8418c8ec655a2083e174aaa385de74d76`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 284.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip
	-	`sha256:0da709e3482cc552b0a7b69eb05aaa21af1e74baaf4e3bccc34e95e478943630`  
		Last Modified: Wed, 13 Dec 2023 00:26:36 GMT  
		Size: 122.0 B  
		MIME: application/vnd.oci.image.layer.v1.tar+gzip

### `memcached:1-bookworm` - unknown; unknown

```console
$ docker pull memcached@sha256:525abad348ba03c5b9444f23409d647581284c1642d30539e2c9943405266f12
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.1 MB (3067303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2e3b551ec9122d039520bbd13bced5b1f5b0d5b1fd9e32c09a1d4536f7af1226`

```dockerfile
```

-	Layers:
	-	`sha256:5cc0958f61715f0746d9fa2a8a5c06f31608bb5d1cf32d606c46fc8e11b35984`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 3.0 MB (3046353 bytes)  
		MIME: application/vnd.in-toto+json
	-	`sha256:3d2fed99d3355e42a820c1975105411eb7584cffb111d7e1fd541603f7721f1c`  
		Last Modified: Wed, 13 Dec 2023 00:26:35 GMT  
		Size: 20.9 KB (20950 bytes)  
		MIME: application/vnd.in-toto+json
