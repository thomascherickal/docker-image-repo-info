## `varnish:old-alpine`

```console
$ docker pull varnish@sha256:941ec01f583c63900b2dee0476864d71a2f7876ffd58ca1df55f6913b8832307
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v7
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `varnish:old-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:4dd538daf687c83e08aa11ed141844a6d420630da3e66c7d04442f889c0470b7
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.0 MB (57975575 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e611282d44311df5fe42b44acb581d84377c6b91c8f55d93a7878f97835eb402`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 15:19:26 GMT
ADD file:8ec3735d4b1b4b070607b94e3bd360117b07dc26e1baf5dd485b49b3413e8fff in / 
# Thu, 17 Mar 2022 15:19:26 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 06:18:02 GMT
ENV VARNISH_SIZE=100M
# Fri, 18 Mar 2022 06:20:38 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"8fa163678e2e454fcc959ba24f349de00e6c00357df55f37f12f0d3acbcb2799b2f376385cef2d40c14a4cc44a5eea1b5a3fbf6245961611d4fc3ea30699035d  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Fri, 18 Mar 2022 06:20:39 GMT
WORKDIR /etc/varnish
# Fri, 18 Mar 2022 06:20:39 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Fri, 18 Mar 2022 06:20:39 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 18 Mar 2022 06:20:39 GMT
EXPOSE 80 8443
# Fri, 18 Mar 2022 06:20:40 GMT
CMD []
```

-	Layers:
	-	`sha256:36ccefbf3d8a9a1b18baaa9cbf0f3ad50e8a7b751656c74df359900a318cbffc`  
		Last Modified: Thu, 17 Mar 2022 15:20:13 GMT  
		Size: 2.8 MB (2816169 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4f0763a8d464814e6b1206cefd228fbadef51486477e41d5cf634caa9babb5b0`  
		Last Modified: Fri, 18 Mar 2022 06:22:43 GMT  
		Size: 55.2 MB (55158700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fbf1b9dfbed74e6d13e8a424b2fe714c0cedf7612baf786b20ac19967bd9cbc8`  
		Last Modified: Fri, 18 Mar 2022 06:22:34 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm variant v7

```console
$ docker pull varnish@sha256:31053b247eb635379c95b41e983e33594f546d89ffab66d9b7126b54aa250e46
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **43.8 MB (43817481 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:625d7d634e6276744e6b233ed4b00bd080b0261c530e52dbd389bfde3d2b3655`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 12 Nov 2021 16:57:35 GMT
ADD file:03e0720458c3475758bf4394afa56f2165198eb91e6e9581f7768e433744dd9b in / 
# Fri, 12 Nov 2021 16:57:36 GMT
CMD ["/bin/sh"]
# Sat, 13 Nov 2021 15:41:33 GMT
ENV VARNISH_SIZE=100M
# Wed, 26 Jan 2022 01:12:26 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"8fa163678e2e454fcc959ba24f349de00e6c00357df55f37f12f0d3acbcb2799b2f376385cef2d40c14a4cc44a5eea1b5a3fbf6245961611d4fc3ea30699035d  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Wed, 26 Jan 2022 01:12:27 GMT
WORKDIR /etc/varnish
# Wed, 26 Jan 2022 01:12:28 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Wed, 26 Jan 2022 01:12:28 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Wed, 26 Jan 2022 01:12:28 GMT
EXPOSE 80 8443
# Wed, 26 Jan 2022 01:12:29 GMT
CMD []
```

-	Layers:
	-	`sha256:764d2e53e1a607f2d8261522185d5b9021ade3ec1a595664ee90308c00176899`  
		Last Modified: Fri, 12 Nov 2021 16:59:33 GMT  
		Size: 2.4 MB (2438618 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2a5e549228b5c5abf70a9698b4aba7a7583a13026844c09b26a24fed89b7e7b`  
		Last Modified: Wed, 26 Jan 2022 01:16:43 GMT  
		Size: 41.4 MB (41378155 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d4e6607ab940d987c29b58e1ebcc2645cf6fd0f612c076ff86756b0f1e4315e`  
		Last Modified: Wed, 26 Jan 2022 01:16:22 GMT  
		Size: 708.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; arm64 variant v8

```console
$ docker pull varnish@sha256:b76b959a3956e1519ff47eac8539024869f120a9b2df48746279e059911097e3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.7 MB (50732237 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f175b35d4b8fc6e3dbef75446e9921b143be0310e79dca19e6ae353615c0d71a`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 18:43:12 GMT
ADD file:611998b78638b13e78919dd4635674032ab233f9b7aae6f62beaf6634cd18b9e in / 
# Thu, 17 Mar 2022 18:43:13 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:11:46 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 21:15:53 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"8fa163678e2e454fcc959ba24f349de00e6c00357df55f37f12f0d3acbcb2799b2f376385cef2d40c14a4cc44a5eea1b5a3fbf6245961611d4fc3ea30699035d  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Thu, 17 Mar 2022 21:15:53 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 21:15:55 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:15:55 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 21:15:56 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 21:15:57 GMT
CMD []
```

-	Layers:
	-	`sha256:93a1719cf26168d3a85db2594d76b17ccc4b25996620bceed3c2a13eaa165325`  
		Last Modified: Thu, 17 Mar 2022 18:44:00 GMT  
		Size: 2.7 MB (2715888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe85643f52ba4cfd1b4f9a57ea726b9a40fe552f48d5d5538e2cc73d1ff33550`  
		Last Modified: Thu, 17 Mar 2022 21:20:28 GMT  
		Size: 48.0 MB (48015639 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eeb2e5a6b4d8fd62f4c3d59d85e5a518f0fbe572f7ff09e6c4a7529e02c4c6c`  
		Last Modified: Thu, 17 Mar 2022 21:20:21 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; 386

```console
$ docker pull varnish@sha256:b74be8a174e7e4d86d620842aeee0bf2ac2d45632733cac4c66db12d4c1c17ac
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.2 MB (58181203 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:df9be027a4ac94114a30966b952c0d4afd3ffc44a693257c7e6a51fc5593ce75`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 16:34:36 GMT
ADD file:5bb8a2cf301e0add52528df0f7f5c5b3c9b14495c5aa85c8fd628731fcd348aa in / 
# Thu, 17 Mar 2022 16:34:36 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 21:45:52 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 21:49:28 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"8fa163678e2e454fcc959ba24f349de00e6c00357df55f37f12f0d3acbcb2799b2f376385cef2d40c14a4cc44a5eea1b5a3fbf6245961611d4fc3ea30699035d  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Thu, 17 Mar 2022 21:49:29 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 21:49:29 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 17 Mar 2022 21:49:29 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 21:49:29 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 21:49:30 GMT
CMD []
```

-	Layers:
	-	`sha256:8fd9b2c548e42517da6865245538c8f53b774738b4fd7cb2d57ad8716e71748c`  
		Last Modified: Thu, 17 Mar 2022 16:35:25 GMT  
		Size: 2.8 MB (2823782 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac571b6fa23815c55ac6eef1364b03088012b0d8a27624052bf1728b11a318c7`  
		Last Modified: Thu, 17 Mar 2022 21:52:49 GMT  
		Size: 55.4 MB (55356713 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5724fb835c6acb0a3fc58cf23bdab3d5774e69115048122e450bc4a61d539468`  
		Last Modified: Thu, 17 Mar 2022 21:52:33 GMT  
		Size: 708.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; ppc64le

```console
$ docker pull varnish@sha256:fb49e9d771ea3b6e2c2f71158182235ebaf45a1a5d659969a33cbae0ca7b1c66
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **47.8 MB (47818289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3328db077f259bbc4ca1c325a4fff35c178a78578b08121197b1b3a7b78cd0de`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 18:18:43 GMT
ADD file:bf9c99d8209e0bed9fd3b62cbe691ebf3829d5a35e63e2b066f1f842577a6d24 in / 
# Thu, 17 Mar 2022 18:18:48 GMT
CMD ["/bin/sh"]
# Fri, 18 Mar 2022 12:09:18 GMT
ENV VARNISH_SIZE=100M
# Fri, 18 Mar 2022 12:13:03 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"8fa163678e2e454fcc959ba24f349de00e6c00357df55f37f12f0d3acbcb2799b2f376385cef2d40c14a4cc44a5eea1b5a3fbf6245961611d4fc3ea30699035d  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Fri, 18 Mar 2022 12:13:09 GMT
WORKDIR /etc/varnish
# Fri, 18 Mar 2022 12:13:18 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Fri, 18 Mar 2022 12:13:34 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Fri, 18 Mar 2022 12:13:46 GMT
EXPOSE 80 8443
# Fri, 18 Mar 2022 12:13:55 GMT
CMD []
```

-	Layers:
	-	`sha256:8b7e8363a93630a772b70e3cf72231f43c62addae0ee8e507c61d43e3781c4e7`  
		Last Modified: Thu, 17 Mar 2022 18:20:01 GMT  
		Size: 2.8 MB (2817281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7937e12c2add4536f3f69d9dcfbdc34f8a8b236e2f055d3e549a039b0e7e9be3`  
		Last Modified: Fri, 18 Mar 2022 12:17:19 GMT  
		Size: 45.0 MB (45000298 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:108ba8575e8988b645875f627f3de0c34b38f85e399683805b9b1e4a02ce839e`  
		Last Modified: Fri, 18 Mar 2022 12:17:10 GMT  
		Size: 710.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `varnish:old-alpine` - linux; s390x

```console
$ docker pull varnish@sha256:1f23309d9e05bc2c44fcac6cb0dcb1aa17e9bd56cae997b96cdceb5b9e9b284a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **46.3 MB (46347687 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:014c4076e1b7a6e9f81ab52b4664e7f4cc914faed84d5fe4c4300649fe8d352f`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Thu, 17 Mar 2022 14:35:54 GMT
ADD file:cd4f7409c75ce2e40b46bbdeca277e2c4500aab51e1a7b6fa518c60e371f0a33 in / 
# Thu, 17 Mar 2022 14:35:55 GMT
CMD ["/bin/sh"]
# Thu, 17 Mar 2022 16:53:33 GMT
ENV VARNISH_SIZE=100M
# Thu, 17 Mar 2022 16:57:10 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout d3e6a3fad7d4c2ac781ada92dcc246e7eef9d129;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.2/" 	-e 's@^source=.*@source="https://varnish-cache.org/downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"8fa163678e2e454fcc959ba24f349de00e6c00357df55f37f12f0d3acbcb2799b2f376385cef2d40c14a4cc44a5eea1b5a3fbf6245961611d4fc3ea30699035d  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder;
# Thu, 17 Mar 2022 16:57:12 GMT
WORKDIR /etc/varnish
# Thu, 17 Mar 2022 16:57:12 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Thu, 17 Mar 2022 16:57:12 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Thu, 17 Mar 2022 16:57:12 GMT
EXPOSE 80 8443
# Thu, 17 Mar 2022 16:57:12 GMT
CMD []
```

-	Layers:
	-	`sha256:1a9a9eea18bd912112f7ed42a3730393bafbb84387ab6790fe9358d09100f3a3`  
		Last Modified: Thu, 17 Mar 2022 14:36:47 GMT  
		Size: 2.6 MB (2605208 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b1acd94f2e87808566fe047b38c94f35a6aa54af1469198a85cc24a0cfb0e99`  
		Last Modified: Thu, 17 Mar 2022 16:59:17 GMT  
		Size: 43.7 MB (43741773 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:35e4d9c7c3e48c5b262143c033346bf32ddd9eba8fbba661e561d1d6a584fb41`  
		Last Modified: Thu, 17 Mar 2022 16:59:11 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
