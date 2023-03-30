## `api-firewall:latest`

```console
$ docker pull api-firewall@sha256:9c6d289ef4b7396c229afa1f1a49ee6111edf9213348f4c989afa9d4292a430a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 3
	-	linux; amd64
	-	linux; arm64 variant v8
	-	linux; 386

### `api-firewall:latest` - linux; amd64

```console
$ docker pull api-firewall@sha256:034b3292ce4aa149a6cff097e2b9fc58bba2ce1e00c6b4645cabb030c5b52aab
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **9.0 MB (8982910 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7e38530f647b5d3ba25cba838b86300f8700f4a87f0c72c02945dc7bd5a8a0e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Wed, 29 Mar 2023 18:19:24 GMT
ADD file:9a4f77dfaba7fd2aa78186e4ef0e7486ad55101cefc1fabbc1b385601bb38920 in / 
# Wed, 29 Mar 2023 18:19:24 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:33:23 GMT
ENV APIFW_PATH=/opt/api-firewall
# Wed, 29 Mar 2023 19:33:24 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 19:33:24 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Wed, 29 Mar 2023 19:33:24 GMT
ENV APIFIREWALL_VERSION=v0.6.11
# Wed, 29 Mar 2023 19:33:27 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='c76cdb6c6185038ea619e364acc71066831de85aefe7e32f8fdbdcc110125cc1';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='786b645dd11cb34ce2ee512b1f75b8929095e25de0027bff5817dedc895eb883';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='351af5ba7af8a010c941416f863bfd52d3e4f04f6ebba77cdf388c37b39e7c75';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Wed, 29 Mar 2023 19:33:27 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Wed, 29 Mar 2023 19:33:27 GMT
USER api-firewall
# Wed, 29 Mar 2023 19:33:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:33:27 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:f56be85fc22e46face30e2c3de3f7fe7c15f8fd7c4e5add29d7f64b87abdaa09`  
		Last Modified: Wed, 29 Mar 2023 18:19:57 GMT  
		Size: 3.4 MB (3374563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:085aa53bc6dba091a419b6c3e1f745a1748914575dca4114e1003fac0fdb0938`  
		Last Modified: Wed, 29 Mar 2023 19:33:44 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af23408db57eb594b9ee9b7d3fa611016f3e0d53e2e8e5ac78ef7381b501e1d2`  
		Last Modified: Wed, 29 Mar 2023 19:33:45 GMT  
		Size: 5.6 MB (5606792 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67872c68496533df2c11048e1059194bc373470daa17890ef72b6846018a7270`  
		Last Modified: Wed, 29 Mar 2023 19:33:44 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:latest` - linux; arm64 variant v8

```console
$ docker pull api-firewall@sha256:1c55ed778f684fe3f46b0f622bac2748b7f32821d1e7bc97012f4cf5ebd4c0d1
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.5 MB (8491503 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e656e2c81969da40f66aededa5d1b4c48bdbe2616010ad15b579528bc65918dc`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Wed, 29 Mar 2023 17:39:18 GMT
ADD file:e51d4089e73ad6dee52b31f0c8059a00c17df6e23f6741fe11b43bd84cc99008 in / 
# Wed, 29 Mar 2023 17:39:18 GMT
CMD ["/bin/sh"]
# Thu, 30 Mar 2023 03:34:53 GMT
ENV APIFW_PATH=/opt/api-firewall
# Thu, 30 Mar 2023 03:34:53 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Thu, 30 Mar 2023 03:34:54 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Thu, 30 Mar 2023 03:34:54 GMT
ENV APIFIREWALL_VERSION=v0.6.11
# Thu, 30 Mar 2023 03:34:55 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='c76cdb6c6185038ea619e364acc71066831de85aefe7e32f8fdbdcc110125cc1';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='786b645dd11cb34ce2ee512b1f75b8929095e25de0027bff5817dedc895eb883';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='351af5ba7af8a010c941416f863bfd52d3e4f04f6ebba77cdf388c37b39e7c75';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Thu, 30 Mar 2023 03:34:56 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Thu, 30 Mar 2023 03:34:56 GMT
USER api-firewall
# Thu, 30 Mar 2023 03:34:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 30 Mar 2023 03:34:56 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:c41833b44d910632b415cd89a9cdaa4d62c9725dc56c99a7ddadafd6719960f9`  
		Last Modified: Wed, 29 Mar 2023 17:39:44 GMT  
		Size: 3.3 MB (3261854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d84d7c1ba39363b27c3da9c1fe8f98fea646963d2c2be490db471022adddcb88`  
		Last Modified: Thu, 30 Mar 2023 03:35:10 GMT  
		Size: 1.2 KB (1200 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:374a9e5b132ddedc68ce8b9123a60bc27d231510071a895300e0e1decf7feb13`  
		Last Modified: Thu, 30 Mar 2023 03:35:11 GMT  
		Size: 5.2 MB (5228095 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ac4c0c64f5c31c8de78705d7807b5b5a29239650e66820dc561b38c6dfdc519`  
		Last Modified: Thu, 30 Mar 2023 03:35:10 GMT  
		Size: 354.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `api-firewall:latest` - linux; 386

```console
$ docker pull api-firewall@sha256:d3138561a5682a0675f13cba44a2be3d97cc6ea6a1e87007d4605ab091fa3f99
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **8.9 MB (8878913 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:812df08e1f395951a453a224323c1089001b523fcfbb8cc6b22677822633e214`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["api-firewall"]`

```dockerfile
# Wed, 29 Mar 2023 17:38:30 GMT
ADD file:61bc44c9685b610d18bddd05d2ea1e57b4313f5f433a0a0b7e5269ec24f108b0 in / 
# Wed, 29 Mar 2023 17:38:30 GMT
CMD ["/bin/sh"]
# Wed, 29 Mar 2023 19:17:56 GMT
ENV APIFW_PATH=/opt/api-firewall
# Wed, 29 Mar 2023 19:17:56 GMT
ENV PATH=/opt/api-firewall:/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin
# Wed, 29 Mar 2023 19:17:57 GMT
RUN set -eux;     adduser -u 1000 -H -h /opt -D -s /bin/sh api-firewall
# Wed, 29 Mar 2023 19:17:57 GMT
ENV APIFIREWALL_VERSION=v0.6.11
# Wed, 29 Mar 2023 19:17:59 GMT
RUN set -eux;         apk add --no-cache wget;         arch="$(apk --print-arch)";     case "$arch" in         'x86_64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-amd64-musl.tar.gz";             sha256='c76cdb6c6185038ea619e364acc71066831de85aefe7e32f8fdbdcc110125cc1';             ;;         'aarch64')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-arm64-musl.tar.gz";             sha256='786b645dd11cb34ce2ee512b1f75b8929095e25de0027bff5817dedc895eb883';             ;;         'x86')             url="https://github.com/wallarm/api-firewall/releases/download/${APIFIREWALL_VERSION}/api-firewall-386-musl.tar.gz";             sha256='351af5ba7af8a010c941416f863bfd52d3e4f04f6ebba77cdf388c37b39e7c75';             ;;         *)             echo >&2 "error: current architecture ($arch) does not have a corresponding API-Firewall binary release";             exit 1;             ;;     esac;         wget -O api-firewall.tar.gz "$url";     echo "$sha256 *api-firewall.tar.gz" | sha256sum -c;         mkdir -p "$APIFW_PATH";     tar -xzf api-firewall.tar.gz -C "$APIFW_PATH" --strip-components 1;     rm api-firewall.tar.gz;         chmod 755 $APIFW_PATH/api-firewall;         api-firewall -v
# Wed, 29 Mar 2023 19:17:59 GMT
COPY file:d278e8d8f9cc8e98b02127f87703b4379a8a938a57e107aac5dd34c716907f87 in /opt/api-firewall/ 
# Wed, 29 Mar 2023 19:17:59 GMT
USER api-firewall
# Wed, 29 Mar 2023 19:18:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 29 Mar 2023 19:18:00 GMT
CMD ["api-firewall"]
```

-	Layers:
	-	`sha256:b2b0f0faedf1b87a3c77cf90d027fb7a25aa67f35400244a4655ad5842a757e4`  
		Last Modified: Wed, 29 Mar 2023 17:39:00 GMT  
		Size: 3.4 MB (3412260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3dcc6ef49f75790d9a4fb6684238589d6fc72825a48cda0434f5722341357027`  
		Last Modified: Wed, 29 Mar 2023 19:18:17 GMT  
		Size: 1.2 KB (1201 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d704a7e1675f0bb9d3a68d49137a870d0d38a59f79bca9c450fe94cb377e483`  
		Last Modified: Wed, 29 Mar 2023 19:18:18 GMT  
		Size: 5.5 MB (5465099 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf7b31015c4f49667a96a8a7b5935e6e23a8b5d85d6849de025e398520732753`  
		Last Modified: Wed, 29 Mar 2023 19:18:17 GMT  
		Size: 353.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
