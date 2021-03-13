## `vault:latest`

```console
$ docker pull vault@sha256:17e587f3475d67cca24451848bd0ea69989fe48c18eee226d3a48db3b6aa44f5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:8ef538af66967e784a7b0b32efa8c6473365194c81c3a5d717e831dd5cab9155
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68982863 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:83d03b2b783e9a59abae959dd6e6c7a5ccaf9f0cf9793d8efa5ee9d699170ed3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 11:42:02 GMT
ARG VAULT_VERSION=1.6.3
# Sat, 13 Mar 2021 11:42:03 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 13 Mar 2021 11:42:10 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 13 Mar 2021 11:42:11 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 13 Mar 2021 11:42:11 GMT
VOLUME [/vault/logs]
# Sat, 13 Mar 2021 11:42:11 GMT
VOLUME [/vault/file]
# Sat, 13 Mar 2021 11:42:12 GMT
EXPOSE 8200
# Sat, 13 Mar 2021 11:42:12 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Mar 2021 11:42:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 11:42:12 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebf90fe65cc1210aaa1cb21c2ef7e703360fbc3ca31c3d62f2662764c3c32138`  
		Last Modified: Sat, 13 Mar 2021 11:43:07 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:479c1be4a4052222497832548909cb2f5f71983ed9657a6d65499427be8f371f`  
		Last Modified: Sat, 13 Mar 2021 11:43:16 GMT  
		Size: 66.2 MB (66167936 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8987a40e7560c149aebe107febfac483c7e83c593647f782b9521255bd60fdd6`  
		Last Modified: Sat, 13 Mar 2021 11:43:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:982296b02bf83c568505556c537de0f55e3a951c2c000aa06ed179200bfcb8ac`  
		Last Modified: Sat, 13 Mar 2021 11:43:06 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:c259ca51167c63aa9607d919b2c55db9eb7b7a78f71e451da595a562e7481760
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63718893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b12efd0b4318752f6ee120b58288113977130db7a2d1859621b3130c6c5e1c96`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 23:14:53 GMT
ARG VAULT_VERSION=1.6.3
# Tue, 02 Mar 2021 23:14:54 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 02 Mar 2021 23:15:06 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 02 Mar 2021 23:15:09 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 02 Mar 2021 23:15:10 GMT
VOLUME [/vault/logs]
# Tue, 02 Mar 2021 23:15:11 GMT
VOLUME [/vault/file]
# Tue, 02 Mar 2021 23:15:12 GMT
EXPOSE 8200
# Tue, 02 Mar 2021 23:15:12 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Mar 2021 23:15:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 23:15:14 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:565cbb62e6435fa12e134fa98dd06c89e72cb48235f763bc4d730d144cc7a1f8`  
		Last Modified: Tue, 02 Mar 2021 23:15:36 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:284162887dd90cdadae098858307a49f9d62bdd19a07dd1c13918486d4713703`  
		Last Modified: Tue, 02 Mar 2021 23:15:52 GMT  
		Size: 61.1 MB (61093587 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65b4c9ad70bb6e855693e16c1a7108c23673a58ff4897b17b3b19282ec14ed02`  
		Last Modified: Tue, 02 Mar 2021 23:15:36 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51322c75e1e50cf02683375fbc23aa2288d8dd6af7d4a84029a7c142f4749ad5`  
		Last Modified: Tue, 02 Mar 2021 23:15:36 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:f6f42cfae7bb0e4db405930b85246960388b493598296e32216006a25895b490
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (65015972 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9db3e6d5cd58d59e467cc2628643c5c49080a729b8a28c047f4a3361fe0610ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 20:39:29 GMT
ADD file:3bf1497bd250cf7c73c12231dc4ebe3a3a67f2cd99e35bce47ef6674683aeb1d in / 
# Wed, 17 Feb 2021 20:39:30 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 23:00:04 GMT
ARG VAULT_VERSION=1.6.3
# Tue, 02 Mar 2021 23:00:07 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 02 Mar 2021 23:00:21 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 02 Mar 2021 23:00:24 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 02 Mar 2021 23:00:25 GMT
VOLUME [/vault/logs]
# Tue, 02 Mar 2021 23:00:25 GMT
VOLUME [/vault/file]
# Tue, 02 Mar 2021 23:00:27 GMT
EXPOSE 8200
# Tue, 02 Mar 2021 23:00:28 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Mar 2021 23:00:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 23:00:30 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:069a56d6d07f6b186fbb82e4486616b9be9a37ce32a63013af6cddcb65898182`  
		Last Modified: Wed, 17 Feb 2021 20:40:04 GMT  
		Size: 2.7 MB (2711572 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f28d5e0abd1f586bd1f92372c7bd965218df4b3388ea881f7c0ea48f134c4ac`  
		Last Modified: Tue, 02 Mar 2021 23:00:59 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea3d060932ea51ab17f91ef330c219bb2e6c99bd2db6454b557d401c15438d0`  
		Last Modified: Tue, 02 Mar 2021 23:01:12 GMT  
		Size: 62.3 MB (62301132 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a8efb2df7982195004f1be44691579ab5fc37954dcf8ae84a6520904e417fcf`  
		Last Modified: Tue, 02 Mar 2021 23:01:00 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd7243d4f0f132c177a143c28a1854bdbf7911defe968cee4f4235698bad712b`  
		Last Modified: Tue, 02 Mar 2021 23:01:00 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:c88f2267f674e946cda289fe4ca74e08b020df367d5794079ddb5697993507ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67033174 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eb4690e8d201f8da8e9156bc6aaddd0fd70be06fbc0e104f51f449199ec53f7f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 21:38:34 GMT
ADD file:eaee53da3c87749799de55809e4a5b526c56855332b961a85b1184c660f1d65b in / 
# Wed, 17 Feb 2021 21:38:35 GMT
CMD ["/bin/sh"]
# Sat, 13 Mar 2021 04:20:39 GMT
ARG VAULT_VERSION=1.6.3
# Sat, 13 Mar 2021 04:20:39 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 13 Mar 2021 04:20:47 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 13 Mar 2021 04:20:48 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 13 Mar 2021 04:20:48 GMT
VOLUME [/vault/logs]
# Sat, 13 Mar 2021 04:20:49 GMT
VOLUME [/vault/file]
# Sat, 13 Mar 2021 04:20:49 GMT
EXPOSE 8200
# Sat, 13 Mar 2021 04:20:49 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 13 Mar 2021 04:20:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 13 Mar 2021 04:20:49 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:86205afa28f6bc624469015a543d16608258d2828411a92c662f4fdc6d276e18`  
		Last Modified: Wed, 17 Feb 2021 21:39:07 GMT  
		Size: 2.8 MB (2818177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e4e2efb828c20a20c7e10f0e0d5ad91c51d9d287e583c699ea0f71c618ad24c`  
		Last Modified: Sat, 13 Mar 2021 04:22:02 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ede3b452c48602c7f834022bf8eb76e66acb650c25659a3a2502346ffa46af6`  
		Last Modified: Sat, 13 Mar 2021 04:22:12 GMT  
		Size: 64.2 MB (64211731 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ecb4bcc937a3d8ed95c0cfac11c12b349557d4d0b78e6bb5f26c116549971c58`  
		Last Modified: Sat, 13 Mar 2021 04:22:02 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23fcb17f032c6add01d605cca0b8b53a075bafff6cd254c40eca88402865fc4`  
		Last Modified: Sat, 13 Mar 2021 04:22:02 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
