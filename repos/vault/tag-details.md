<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.3.1`](#vault131)
-	[`vault:latest`](#vaultlatest)

## `vault:1.3.1`

```console
$ docker pull vault@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `vault:latest`

```console
$ docker pull vault@sha256:2879f79ffccca39772b86a6e3e001c2d398b729b7b501a1d3e7abb8e80b80444
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:0d67bf30e7b1df4a74c7a89e5e3e80f6956417c4962bbda0a8e5472d3766b671
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51625754 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dae6e7a2e6ec69721962e779e8291212cf85f79b1e594c966e7605c7d54dae3d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Thu, 14 Nov 2019 22:21:23 GMT
ARG VAULT_VERSION=1.3.0
# Thu, 14 Nov 2019 22:21:24 GMT
# ARGS: VAULT_VERSION=1.3.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 14 Nov 2019 22:21:29 GMT
# ARGS: VAULT_VERSION=1.3.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 14 Nov 2019 22:21:30 GMT
# ARGS: VAULT_VERSION=1.3.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 14 Nov 2019 22:21:30 GMT
VOLUME [/vault/logs]
# Thu, 14 Nov 2019 22:21:30 GMT
VOLUME [/vault/file]
# Thu, 14 Nov 2019 22:21:30 GMT
EXPOSE 8200
# Thu, 14 Nov 2019 22:21:31 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Nov 2019 22:21:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Nov 2019 22:21:31 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d981842b573ad7b465eb7596aca26ba70a76996048ee8b2dd3aa72dc10ae204`  
		Last Modified: Thu, 14 Nov 2019 22:21:38 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c6cb12fcc0c7e5b353a179dfbacc7674c5b5eff4e207e4ac0b210d7d0f2fb19`  
		Last Modified: Thu, 14 Nov 2019 22:21:46 GMT  
		Size: 48.8 MB (48835386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f6830c2dbcfdd251b7b236ba8924e7dfa2fb20f4e633f0af150c629b2734570`  
		Last Modified: Thu, 14 Nov 2019 22:21:38 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c780a4bd3e455d72b4f40cfdc0a61c649cbcd7654f5ec973333a32ef490c3c6c`  
		Last Modified: Thu, 14 Nov 2019 22:21:38 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:776181b9b6f2393268478824876e48ad5708b6a6bab69a3e75bf2d17c4ca5696
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48643743 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4e5c384ed2d74d7197aad147c80701fbd03602cdadceef80c34a2a7996ed9834`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Thu, 14 Nov 2019 21:53:26 GMT
ARG VAULT_VERSION=1.3.0
# Thu, 14 Nov 2019 21:53:30 GMT
# ARGS: VAULT_VERSION=1.3.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 14 Nov 2019 21:53:40 GMT
# ARGS: VAULT_VERSION=1.3.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 14 Nov 2019 21:53:42 GMT
# ARGS: VAULT_VERSION=1.3.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 14 Nov 2019 21:53:43 GMT
VOLUME [/vault/logs]
# Thu, 14 Nov 2019 21:53:44 GMT
VOLUME [/vault/file]
# Thu, 14 Nov 2019 21:53:45 GMT
EXPOSE 8200
# Thu, 14 Nov 2019 21:53:45 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Nov 2019 21:53:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Nov 2019 21:53:47 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f8e1bd31da1797a08e9d8d338db4e912bd4eb7efff4d3f09cadeed831bf4f42c`  
		Last Modified: Thu, 14 Nov 2019 21:53:58 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c060c82612dfa6fdaaa02cf6e1e81606f44d6ac8d72bb5553bb4f120b2708fef`  
		Last Modified: Thu, 14 Nov 2019 21:54:12 GMT  
		Size: 46.1 MB (46069136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:060c7580558250953f040b26ee73d508d2d83e2f67974601d7ee8180b379d8d5`  
		Last Modified: Thu, 14 Nov 2019 21:53:58 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:12d5cddb80839b7d48e20b106db822217fd7f918206cbf518c56cca689f500bf`  
		Last Modified: Thu, 14 Nov 2019 21:53:58 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:ab4c3eaa5e6a79276c24b62d9fd4f427829b06788fa8ec1963c1298756b21618
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48696340 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8ec6724aac3f66156b568e77a5a0d4790bd998a58f3fa0aee6819873f44ca50b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Thu, 14 Nov 2019 21:41:04 GMT
ARG VAULT_VERSION=1.3.0
# Thu, 14 Nov 2019 21:41:06 GMT
# ARGS: VAULT_VERSION=1.3.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 14 Nov 2019 21:41:13 GMT
# ARGS: VAULT_VERSION=1.3.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 14 Nov 2019 21:41:16 GMT
# ARGS: VAULT_VERSION=1.3.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 14 Nov 2019 21:41:17 GMT
VOLUME [/vault/logs]
# Thu, 14 Nov 2019 21:41:17 GMT
VOLUME [/vault/file]
# Thu, 14 Nov 2019 21:41:18 GMT
EXPOSE 8200
# Thu, 14 Nov 2019 21:41:19 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Nov 2019 21:41:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Nov 2019 21:41:20 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a0b2cbc7c3770aaac605f99f0059103a2216fc974dc9df1042f8e920b107f0f`  
		Last Modified: Thu, 14 Nov 2019 21:41:30 GMT  
		Size: 1.3 KB (1285 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46c17cb8d2c803baa454f01c9b7988ead9485c293f2545da87be9f32478d9028`  
		Last Modified: Thu, 14 Nov 2019 21:41:41 GMT  
		Size: 46.0 MB (45975268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2626a85334398b8758c99f22232bd7e48333fd3c5016c0961c4f3c8620f054f8`  
		Last Modified: Thu, 14 Nov 2019 21:41:30 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:73ddcce64f9860de87b9f133e247a0cc3171d2334dc1839845cbc6571007b161`  
		Last Modified: Thu, 14 Nov 2019 21:41:30 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:b49738b8b78ff8046de6b41ae70ee41b29f0cf95485a554b2d949f0eccf77706
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50098494 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:142867dd67f2e1e31c7fa5211d6119340850a37b014d66c6e8a4c2d16b7c54ea`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Mon, 21 Oct 2019 16:46:04 GMT
ADD file:dd3b3676fd9c1e0983ade68242b9b9ac5c477f3e4bfc97c2e78fd5db93a441c9 in / 
# Mon, 21 Oct 2019 16:46:04 GMT
CMD ["/bin/sh"]
# Thu, 14 Nov 2019 21:39:31 GMT
ARG VAULT_VERSION=1.3.0
# Thu, 14 Nov 2019 21:39:31 GMT
# ARGS: VAULT_VERSION=1.3.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 14 Nov 2019 21:39:37 GMT
# ARGS: VAULT_VERSION=1.3.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 14 Nov 2019 21:39:38 GMT
# ARGS: VAULT_VERSION=1.3.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 14 Nov 2019 21:39:38 GMT
VOLUME [/vault/logs]
# Thu, 14 Nov 2019 21:39:38 GMT
VOLUME [/vault/file]
# Thu, 14 Nov 2019 21:39:38 GMT
EXPOSE 8200
# Thu, 14 Nov 2019 21:39:39 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 14 Nov 2019 21:39:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 14 Nov 2019 21:39:39 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f913bd05bf684aaa4bc173d73cfbb58abb45587962d74f0aa71df36b6b489def`  
		Last Modified: Mon, 21 Oct 2019 16:46:25 GMT  
		Size: 2.8 MB (2785939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34abdd77e9b9ca31c6462394238d63d39c60f55f2cf45403a2cd8eaa60f52fd8`  
		Last Modified: Thu, 14 Nov 2019 21:39:47 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6d1d74bd4665a8dcc981294f0a5cd8d55df1ad8d34cc69a3fcbc1c1ab08c0b0`  
		Last Modified: Thu, 14 Nov 2019 21:39:55 GMT  
		Size: 47.3 MB (47309320 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:019954a22515d5d5a4a4bd778f3ffd8b930e954d392ecfeb81067026673bd2d6`  
		Last Modified: Thu, 14 Nov 2019 21:39:47 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b2effc1bf5bb335d742eacbcef4620a9eb6ae02890a372709e3e6c2cc596465d`  
		Last Modified: Thu, 14 Nov 2019 21:39:47 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
