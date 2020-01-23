<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.3.2`](#vault132)
-	[`vault:latest`](#vaultlatest)

## `vault:1.3.2`

```console
$ docker pull vault@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `vault:latest`

```console
$ docker pull vault@sha256:2f797433dfc322d7ba6fa81074e010873c740eb45e83ff5ced49cba585f82a66
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:7f3430debbc28273a73dc0e48e0ea23005fb1b0c5bc39279cc1f8348f09fc7d5
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51633843 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa7801420b956d6febb0e46d75504cec3b2172a5979ff595e41072b2b1f0391d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Mon, 21 Oct 2019 17:21:42 GMT
ADD file:fe1f09249227e2da2089afb4d07e16cbf832eeb804120074acd2b8192876cd28 in / 
# Mon, 21 Oct 2019 17:21:42 GMT
CMD ["/bin/sh"]
# Thu, 19 Dec 2019 04:26:25 GMT
ARG VAULT_VERSION=1.3.1
# Thu, 19 Dec 2019 04:26:26 GMT
# ARGS: VAULT_VERSION=1.3.1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 19 Dec 2019 04:26:32 GMT
# ARGS: VAULT_VERSION=1.3.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 19 Dec 2019 04:26:32 GMT
# ARGS: VAULT_VERSION=1.3.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 19 Dec 2019 04:26:33 GMT
VOLUME [/vault/logs]
# Thu, 19 Dec 2019 04:26:33 GMT
VOLUME [/vault/file]
# Thu, 19 Dec 2019 04:26:33 GMT
EXPOSE 8200
# Thu, 19 Dec 2019 04:26:33 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 04:26:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 04:26:33 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:89d9c30c1d48bac627e5c6cb0d1ed1eec28e7dbdfbcc04712e4c79c0f83faf17`  
		Last Modified: Mon, 21 Oct 2019 17:22:48 GMT  
		Size: 2.8 MB (2787134 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d0e992ffde6d00ca3be22cc6c2ec1b74969b427082e3f6c4cabdec57b6a26d1f`  
		Last Modified: Thu, 19 Dec 2019 04:26:41 GMT  
		Size: 1.3 KB (1258 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3001507ef416214bc7c78138b21c423cb03a14fe84a78808bef5afc90fb2a53f`  
		Last Modified: Thu, 19 Dec 2019 04:26:49 GMT  
		Size: 48.8 MB (48843472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0607b371af8a06ccf1706bca41f750ce84cbb4cac39b689110f5b9ad319825ef`  
		Last Modified: Thu, 19 Dec 2019 04:26:41 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10469b0b103f84202f1ce422b7f68711e1542a40a9286c219c4a598a50005461`  
		Last Modified: Thu, 19 Dec 2019 04:26:41 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:f322481c3a2a84dfa0d041ef0f8b01ba6cb7988626bde5af566d4cb39de73365
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48648976 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c4945fc16b85bbf149082d7d7fb287451cfe9df23de597c7dd98e423f2f087cb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Mon, 21 Oct 2019 16:56:02 GMT
ADD file:d3c7d938a78143f106a6a467ce23b599198e041220e661e5326ba91054c353ef in / 
# Mon, 21 Oct 2019 16:56:04 GMT
CMD ["/bin/sh"]
# Thu, 19 Dec 2019 00:42:52 GMT
ARG VAULT_VERSION=1.3.1
# Thu, 19 Dec 2019 00:42:57 GMT
# ARGS: VAULT_VERSION=1.3.1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 19 Dec 2019 00:43:13 GMT
# ARGS: VAULT_VERSION=1.3.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 19 Dec 2019 00:43:18 GMT
# ARGS: VAULT_VERSION=1.3.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 19 Dec 2019 00:43:23 GMT
VOLUME [/vault/logs]
# Thu, 19 Dec 2019 00:43:25 GMT
VOLUME [/vault/file]
# Thu, 19 Dec 2019 00:43:26 GMT
EXPOSE 8200
# Thu, 19 Dec 2019 00:43:27 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 00:43:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 00:43:30 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:ecf664be551d26dcd221b7387283cdcc54f46c6789700d037fa3cd0c297f8645`  
		Last Modified: Mon, 21 Oct 2019 16:56:34 GMT  
		Size: 2.6 MB (2571309 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca9b20ba6b75d26ea1c4bb8e06d8e3b532e2ddfe863a0252d93d3480b74f1af8`  
		Last Modified: Thu, 19 Dec 2019 00:43:45 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44475e859b93d286a3cefe0cff019c073bca9ef0d0c4d2d186b191fc4fe59897`  
		Last Modified: Thu, 19 Dec 2019 00:44:02 GMT  
		Size: 46.1 MB (46074369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c7f858fd5a1a13b0bf111af7f8c69be894ed88f750f8e8da6325f5284c8c2a79`  
		Last Modified: Thu, 19 Dec 2019 00:43:45 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b7b4473510e5064078ee970208ed5e041e1bb09e983fa113a361390c3fdc08f`  
		Last Modified: Thu, 19 Dec 2019 00:43:46 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:0c11028703dd8707ef2513cccf2886cd1191b7a03dc1b3ab793725938f94a0bb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48705621 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:637ef02b0c7087fcbb5b25af84d48774955bad9b450ffcabfacf1dca659ab45e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Mon, 21 Oct 2019 18:07:03 GMT
ADD file:02f4d68afd9e9e303ff893f198d535d0d78c4b2554f299ab2d0955b2bef0e06a in / 
# Mon, 21 Oct 2019 18:07:09 GMT
CMD ["/bin/sh"]
# Thu, 19 Dec 2019 03:58:15 GMT
ARG VAULT_VERSION=1.3.1
# Thu, 19 Dec 2019 03:58:26 GMT
# ARGS: VAULT_VERSION=1.3.1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 19 Dec 2019 03:58:37 GMT
# ARGS: VAULT_VERSION=1.3.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 19 Dec 2019 03:58:42 GMT
# ARGS: VAULT_VERSION=1.3.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 19 Dec 2019 03:58:43 GMT
VOLUME [/vault/logs]
# Thu, 19 Dec 2019 03:58:44 GMT
VOLUME [/vault/file]
# Thu, 19 Dec 2019 03:58:49 GMT
EXPOSE 8200
# Thu, 19 Dec 2019 03:58:52 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 03:58:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 03:58:54 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8bfa913040406727f36faa9b69d0b96e071b13792a83ad69c19389031a9f3797`  
		Last Modified: Mon, 21 Oct 2019 18:08:36 GMT  
		Size: 2.7 MB (2717778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:003810ed7292d917bc4338a7e84c33e8ff70b29a39fbd45dbce6cf2be6142e93`  
		Last Modified: Thu, 19 Dec 2019 03:59:08 GMT  
		Size: 1.3 KB (1284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:81425b1f1a88c95e95d3d0b71b55bc41b399b7d5dc42a7a47849893345744cc7`  
		Last Modified: Thu, 19 Dec 2019 03:59:21 GMT  
		Size: 46.0 MB (45984548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1692a1f08e7c0bc638d19a3b6f291ed2351f5e74bcc67982c5a58a15cd8f1cd0`  
		Last Modified: Thu, 19 Dec 2019 03:59:08 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc0b398b4a7571e945bbdd5428a6aae8a24b357a0ae47562c884b329d1d7c25d`  
		Last Modified: Thu, 19 Dec 2019 03:59:09 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:2780465a536e5190a336a4bd6943ee1851a4bd9116793fe0a62df2dca59dbeeb
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50106986 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37395a292d457d452cc9a5317958bd28d4cb6b5e92e55b9783519c237d17d0ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Mon, 21 Oct 2019 16:46:04 GMT
ADD file:dd3b3676fd9c1e0983ade68242b9b9ac5c477f3e4bfc97c2e78fd5db93a441c9 in / 
# Mon, 21 Oct 2019 16:46:04 GMT
CMD ["/bin/sh"]
# Thu, 19 Dec 2019 04:49:09 GMT
ARG VAULT_VERSION=1.3.1
# Thu, 19 Dec 2019 04:49:10 GMT
# ARGS: VAULT_VERSION=1.3.1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 19 Dec 2019 04:49:17 GMT
# ARGS: VAULT_VERSION=1.3.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 19 Dec 2019 04:49:18 GMT
# ARGS: VAULT_VERSION=1.3.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 19 Dec 2019 04:49:18 GMT
VOLUME [/vault/logs]
# Thu, 19 Dec 2019 04:49:18 GMT
VOLUME [/vault/file]
# Thu, 19 Dec 2019 04:49:18 GMT
EXPOSE 8200
# Thu, 19 Dec 2019 04:49:19 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 19 Dec 2019 04:49:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 19 Dec 2019 04:49:19 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f913bd05bf684aaa4bc173d73cfbb58abb45587962d74f0aa71df36b6b489def`  
		Last Modified: Mon, 21 Oct 2019 16:46:25 GMT  
		Size: 2.8 MB (2785939 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a8ef6053fe2b5e24e9f9adbac4dc3adb2e88776ddfb34d6c2b90bf4c5350097`  
		Last Modified: Thu, 19 Dec 2019 04:49:27 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:95d4d755b99fcea92d9026a8f5fdf3ee2b0949d67a49aed41ec3e000b79ab881`  
		Last Modified: Thu, 19 Dec 2019 04:49:36 GMT  
		Size: 47.3 MB (47317814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa9dddebe39e51bda232a0ac162727b3008cc8f5c415f9e6066a9a01d0431c29`  
		Last Modified: Thu, 19 Dec 2019 04:49:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7a01bb4d5a3c21d8f280a7a3b042d3386729dc9bd1be17033903791d5387480`  
		Last Modified: Thu, 19 Dec 2019 04:49:27 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
