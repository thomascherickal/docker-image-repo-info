## `varnish:fresh-alpine`

```console
$ docker pull varnish@sha256:5c74f3fca47f1cadd016e5a3acbab74ab1ec531ba2774e02ca482f17825f6487
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `varnish:fresh-alpine` - linux; amd64

```console
$ docker pull varnish@sha256:fb750eb23fab9245a277b8c68fda73e8d2ab47158e77da701a7fea58245c5d55
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **58.0 MB (57979795 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cd8ebd6615c6db4dc111acc75500a60a8b27471ea7e54b64671aa3ca152459d`
-	Entrypoint: `["\/usr\/local\/bin\/docker-varnish-entrypoint"]`
-	Default Command: `[]`

```dockerfile
# Fri, 06 Aug 2021 17:19:45 GMT
ADD file:34eb5c40aa00028921a224d1764ae1b1f3ef710d191e4dfc7df55e0594aa7217 in / 
# Fri, 06 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Sat, 07 Aug 2021 00:26:27 GMT
ENV VARNISH_SIZE=100M
# Sat, 07 Aug 2021 00:27:18 GMT
RUN set -e;    BASE_PKGS="tar alpine-sdk sudo git";     apk add --virtual varnish-build-deps -q --no-progress --update $BASE_PKGS;     git clone https://github.com/varnishcache/pkg-varnish-cache.git;     cd pkg-varnish-cache/alpine;     git checkout 1f139121b5bce0b5b8f5d104224e14880a921b6b;     sed -i APKBUILD         -e "s/pkgver=@VERSION@/pkgver=6.6.1/" 	-e 's@^source=.*@source="http://varnish-cache.org/_downloads/varnish-$pkgver.tgz"@' 	-e "s/^sha512sums=.*/sha512sums=\"af3ee1743af2ede2d3efbb73e5aa9b42c7bbd5f86163ec338c8afd1989c3e51ff3e1b40bed6b72224b5d339a74f22d6e5f3c3faf2fedee8ab4715307ed5d871b  varnish-\$pkgver.tgz\"/";     adduser -D builder;     echo "builder ALL=(ALL) NOPASSWD: ALL" > /etc/sudoers;     addgroup builder abuild;     su builder -c "abuild-keygen -nai";     chown builder -R .;     su builder -c "abuild -r";    apk add --allow-untrusted ~builder/packages/pkg-varnish-cache/*/*.apk;     echo -e 'vcl 4.1;\nbackend default none;' > /etc/varnish/default.vcl;     cp /pkg-varnish-cache/systemd/varnishreload /usr/bin/;     apk del --no-network varnish-build-deps;     rm -rf ~builder /pkg-varnish-cache;     sed -i '/^builder/d' /etc/sudoers;     deluser --remove-home builder
# Sat, 07 Aug 2021 00:27:18 GMT
WORKDIR /etc/varnish
# Sat, 07 Aug 2021 00:27:18 GMT
COPY dir:81cfdf3570a33a2213eb3396395161c2375769c233d0e51a4b70c65b389fabfa in /usr/local/bin/ 
# Sat, 07 Aug 2021 00:27:18 GMT
ENTRYPOINT ["/usr/local/bin/docker-varnish-entrypoint"]
# Sat, 07 Aug 2021 00:27:19 GMT
EXPOSE 80 8443
# Sat, 07 Aug 2021 00:27:19 GMT
CMD []
```

-	Layers:
	-	`sha256:29291e31a76a7e560b9b7ad3cada56e8c18d50a96cca8a2573e4f4689d7aca77`  
		Last Modified: Thu, 05 Aug 2021 15:56:25 GMT  
		Size: 2.8 MB (2813006 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4acc85910e19b26ac30e29972b77ed9dfcbde00f6b6ac65ba59a12c3fecd56d5`  
		Last Modified: Sat, 07 Aug 2021 00:27:52 GMT  
		Size: 55.2 MB (55166083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:90463529b0881c252d0d30e2be3ac057d84874079ac5af714dee1bebdbe2c5e2`  
		Last Modified: Sat, 07 Aug 2021 00:27:44 GMT  
		Size: 706.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
