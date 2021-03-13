<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.4.7`](#vault147)
-	[`vault:1.5.7`](#vault157)
-	[`vault:1.6.3`](#vault163)
-	[`vault:1.7.0-rc1`](#vault170-rc1)
-	[`vault:latest`](#vaultlatest)

## `vault:1.4.7`

```console
$ docker pull vault@sha256:e64e0ab1ba6463efc24a81a58fa0c9d0d8b1f1f8449834b5aa038b9625374dea
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.4.7` - linux; amd64

```console
$ docker pull vault@sha256:4953233b38b47eb65bb4bbbb61efac82a70748d65a272264af3d87fb1edaf3fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52081584 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d76c60b568ae7b3b4469b8fd8a45522dee7351e989cf3913e10dff957e028ab5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:20 GMT
ADD file:74b25a491c5eda6bdc97427d5c0f344be56370a103df816f89ef96052b79a736 in / 
# Wed, 24 Feb 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 03:13:25 GMT
ARG VAULT_VERSION=1.4.7
# Thu, 25 Feb 2021 03:13:26 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 25 Feb 2021 03:13:32 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 25 Feb 2021 03:13:33 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 25 Feb 2021 03:13:33 GMT
VOLUME [/vault/logs]
# Thu, 25 Feb 2021 03:13:33 GMT
VOLUME [/vault/file]
# Thu, 25 Feb 2021 03:13:33 GMT
EXPOSE 8200
# Thu, 25 Feb 2021 03:13:34 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 25 Feb 2021 03:13:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 03:13:34 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8464c5956bbe86052636266c809545517fb2fbc0b945ecc9f0189d73ee1cb0c6`  
		Last Modified: Wed, 24 Feb 2021 20:20:47 GMT  
		Size: 2.8 MB (2797017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88fdcc80801f901b690286b59e9889bbad5af0c39ef5e398961def784a44f155`  
		Last Modified: Thu, 25 Feb 2021 03:14:31 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec192204a692517b220463a7a55ca680cb7c5305ef12c9c45a8ea3a972778fee`  
		Last Modified: Thu, 25 Feb 2021 03:14:41 GMT  
		Size: 49.3 MB (49281331 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8475d9d8e3b32a95303d1cdf9b8e75f8b19dd85b168b77a1fdc35b8956ed8f2`  
		Last Modified: Thu, 25 Feb 2021 03:14:29 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa899944ea207896655d2cf939a52303f231b5d7a4fe360ec861987ae4c48ddb`  
		Last Modified: Thu, 25 Feb 2021 03:14:29 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.7` - linux; arm variant v6

```console
$ docker pull vault@sha256:1d7cdd3157c0730e403268c42b1664c7a12a357fed370a76dc83162e1fb7cd69
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48719706 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0cf464349a93aca1192e4aa9a035dec84f5b917d73df3f0b972c8586b40a73a2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:55 GMT
ADD file:9e81f449863b2d114afc239efa445f3bed6ff45b123ea3aad271a5631ac4fa13 in / 
# Wed, 24 Feb 2021 20:50:56 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:37:59 GMT
ARG VAULT_VERSION=1.4.7
# Wed, 24 Feb 2021 23:38:01 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 24 Feb 2021 23:38:12 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 24 Feb 2021 23:38:14 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 24 Feb 2021 23:38:14 GMT
VOLUME [/vault/logs]
# Wed, 24 Feb 2021 23:38:15 GMT
VOLUME [/vault/file]
# Wed, 24 Feb 2021 23:38:16 GMT
EXPOSE 8200
# Wed, 24 Feb 2021 23:38:16 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 24 Feb 2021 23:38:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:38:18 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:615b6501bf7ed56706d638bf075665f504b2fee0bdebf905dcb8610bc9271fa4`  
		Last Modified: Wed, 24 Feb 2021 20:51:33 GMT  
		Size: 2.6 MB (2574559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c493d5d6dd04e6c618a2a05545ed54f80425ee3ed724bd08f61f6a9a23760fed`  
		Last Modified: Wed, 24 Feb 2021 23:39:21 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:847e00f8e155413726c1399b24fd39855b85c0e5c680cd9899bd4ac4e57b8f6e`  
		Last Modified: Wed, 24 Feb 2021 23:39:33 GMT  
		Size: 46.1 MB (46141854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a89c1e265b041edc4d3e36f1b93cfb8e3670c1453d620ee57fb087b52d9d72ed`  
		Last Modified: Wed, 24 Feb 2021 23:39:21 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faeaa20bf0f90081dc23437718d36e14f3932144e6327241205c897074f3e0a3`  
		Last Modified: Wed, 24 Feb 2021 23:39:21 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.7` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:ac99c0c10f8546fc2d87ce524f4392ab2aa277491760230cde16995d0b3832ef
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48964643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:069d7e1b99400d2b252b1b013f79e519fd8a5007cf00732970e9151384e44b5a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:40:02 GMT
ADD file:422b410b46901dfebf19c61ed06d0bc9931c018b0d96f35da99e4fc409a7776b in / 
# Wed, 24 Feb 2021 20:40:03 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 04:16:25 GMT
ARG VAULT_VERSION=1.4.7
# Thu, 25 Feb 2021 04:16:27 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 25 Feb 2021 04:16:33 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 25 Feb 2021 04:16:36 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 25 Feb 2021 04:16:37 GMT
VOLUME [/vault/logs]
# Thu, 25 Feb 2021 04:16:38 GMT
VOLUME [/vault/file]
# Thu, 25 Feb 2021 04:16:38 GMT
EXPOSE 8200
# Thu, 25 Feb 2021 04:16:39 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 25 Feb 2021 04:16:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 04:16:40 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:1287318d28f14b1b909b2cd8ff908cb037ec28d475bcdf70d1b14fdc0869650f`  
		Last Modified: Wed, 24 Feb 2021 20:40:42 GMT  
		Size: 2.7 MB (2720385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9027e395332ca8325f6a9c3b247306ea693dcadd44b9a28c0fa95a79487f7e4a`  
		Last Modified: Thu, 25 Feb 2021 04:17:43 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9938f9a801a7d4323b4ab271783cda2a32d843a5360d57d7db7f251815dcf32`  
		Last Modified: Thu, 25 Feb 2021 04:17:54 GMT  
		Size: 46.2 MB (46240962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:545582878d948aeedfb9334813af75134816bd89ec1d27364fa712fe9318b681`  
		Last Modified: Thu, 25 Feb 2021 04:17:43 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93bd197544029b70887df308abaee16a9adf0c2f9ce95bd02d09b9a58a210bcd`  
		Last Modified: Thu, 25 Feb 2021 04:17:43 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.7` - linux; 386

```console
$ docker pull vault@sha256:4f76a0ad04b1f6b83f4186497bb42bb82bbb7e15750ad9b9742b14fe53247c1b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50214387 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1358829bba57123e84293125eaf1a27d8396505222731aabcf3f372f72238cf0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:57 GMT
ADD file:b5ef4a4abd9ccb894bdda7a5750878d13fbac4746c7b173c5dc88cf4846fc976 in / 
# Wed, 24 Feb 2021 20:38:57 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:21:49 GMT
ARG VAULT_VERSION=1.4.7
# Thu, 25 Feb 2021 02:21:49 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 25 Feb 2021 02:21:57 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 25 Feb 2021 02:21:57 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 25 Feb 2021 02:21:58 GMT
VOLUME [/vault/logs]
# Thu, 25 Feb 2021 02:21:58 GMT
VOLUME [/vault/file]
# Thu, 25 Feb 2021 02:21:58 GMT
EXPOSE 8200
# Thu, 25 Feb 2021 02:21:58 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 25 Feb 2021 02:21:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:21:59 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:9c18aa22aceabbea5b9c3d26c1e449591c02413fb34b574d9f73520f3fea602b`  
		Last Modified: Wed, 24 Feb 2021 20:39:36 GMT  
		Size: 2.8 MB (2788780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:220fe3fe2a248b7bbddef3b57a8333e8349c3a4f2b4b8088465570dd607e42b3`  
		Last Modified: Thu, 25 Feb 2021 02:22:47 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f33503eda2cab545d58e547471cc38acbbbfc1b0dcb109c15dc189bcc678121`  
		Last Modified: Thu, 25 Feb 2021 02:22:57 GMT  
		Size: 47.4 MB (47422372 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51623e219e50b3126c59ef2ed6f621991b25c868e5a7e34453816463b5a09c14`  
		Last Modified: Thu, 25 Feb 2021 02:22:47 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6583fe4c5d9d6fb03f4bd839494880a2eba1d286db9234b05aa9972ae6186c8d`  
		Last Modified: Thu, 25 Feb 2021 02:22:47 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.5.7`

```console
$ docker pull vault@sha256:5890f84c20a93275346fe250dc7f26f6ad7a54ea732e3fa43635faa88df76df9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.5.7` - linux; amd64

```console
$ docker pull vault@sha256:1760ca0c2f4b87ff8481d9a9ce22642febe1dc8fac25a4abd83ee4fa212274cf
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55009661 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9e629c5680d812897e0625a34f51fa8f2b692c86cfb19267753fc0815c9ec31d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:20:20 GMT
ADD file:74b25a491c5eda6bdc97427d5c0f344be56370a103df816f89ef96052b79a736 in / 
# Wed, 24 Feb 2021 20:20:20 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 03:13:11 GMT
ARG VAULT_VERSION=1.5.7
# Thu, 25 Feb 2021 03:13:12 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 25 Feb 2021 03:13:17 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 25 Feb 2021 03:13:18 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 25 Feb 2021 03:13:19 GMT
VOLUME [/vault/logs]
# Thu, 25 Feb 2021 03:13:19 GMT
VOLUME [/vault/file]
# Thu, 25 Feb 2021 03:13:19 GMT
EXPOSE 8200
# Thu, 25 Feb 2021 03:13:19 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 25 Feb 2021 03:13:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 03:13:20 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8464c5956bbe86052636266c809545517fb2fbc0b945ecc9f0189d73ee1cb0c6`  
		Last Modified: Wed, 24 Feb 2021 20:20:47 GMT  
		Size: 2.8 MB (2797017 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23143b1135d82a338372ef75028022de8b3b53383bf0c539a8f85abfbb1fa21d`  
		Last Modified: Thu, 25 Feb 2021 03:14:13 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27ab78edb80c7dc8b325ed47bce5610074efb06ee9f8e5229ac96175a4172cf`  
		Last Modified: Thu, 25 Feb 2021 03:14:24 GMT  
		Size: 52.2 MB (52209409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ce04aaf95ac993365339a12cb9ef9a87552ac4420eb7616fa398920cd2fce145`  
		Last Modified: Thu, 25 Feb 2021 03:14:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:960707b6567b0c0424b39df75f113214dbd27ac8a3075f9f9e935ce371bd9aab`  
		Last Modified: Thu, 25 Feb 2021 03:14:13 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.7` - linux; arm variant v6

```console
$ docker pull vault@sha256:29e18e929a36011901973283bd4fb7c0723fa8605f3ce60c99f6089134821831
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51563428 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5ebecacf8c1f7878517a0bdfc9b313dd3efcd661daaedcf07817766e44f70b20`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:55 GMT
ADD file:9e81f449863b2d114afc239efa445f3bed6ff45b123ea3aad271a5631ac4fa13 in / 
# Wed, 24 Feb 2021 20:50:56 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:37:28 GMT
ARG VAULT_VERSION=1.5.7
# Wed, 24 Feb 2021 23:37:29 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 24 Feb 2021 23:37:39 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 24 Feb 2021 23:37:42 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 24 Feb 2021 23:37:43 GMT
VOLUME [/vault/logs]
# Wed, 24 Feb 2021 23:37:45 GMT
VOLUME [/vault/file]
# Wed, 24 Feb 2021 23:37:47 GMT
EXPOSE 8200
# Wed, 24 Feb 2021 23:37:48 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 24 Feb 2021 23:37:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:37:50 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:615b6501bf7ed56706d638bf075665f504b2fee0bdebf905dcb8610bc9271fa4`  
		Last Modified: Wed, 24 Feb 2021 20:51:33 GMT  
		Size: 2.6 MB (2574559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:427a2d6e45231426c91f9a0a1944ac81ffce942376ba018cf400b75504c49268`  
		Last Modified: Wed, 24 Feb 2021 23:39:00 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:045524ab01e984686b84e13032ffbe082a603d939306b8d85c959d0f51952e27`  
		Last Modified: Wed, 24 Feb 2021 23:39:14 GMT  
		Size: 49.0 MB (48985575 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6aa1c5eae8a4aebc90bd1d179561f8b161f59f5c282b09c484816f4484fa381`  
		Last Modified: Wed, 24 Feb 2021 23:39:00 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78833d0facb3234c90ed9bfe36fd6249bfe5f6f4523b017380487df1a390c0b`  
		Last Modified: Wed, 24 Feb 2021 23:39:00 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.7` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:aed9a19f1a7ebae87e4d59d6f382004b88dcd850ad528bf6fa4f7f84b11dc861
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51918023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c10f48753ca2a05d1005e5e97ea9a7a04f55222819690bb333618761c4fa0107`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:40:02 GMT
ADD file:422b410b46901dfebf19c61ed06d0bc9931c018b0d96f35da99e4fc409a7776b in / 
# Wed, 24 Feb 2021 20:40:03 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 04:16:01 GMT
ARG VAULT_VERSION=1.5.7
# Thu, 25 Feb 2021 04:16:03 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 25 Feb 2021 04:16:10 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 25 Feb 2021 04:16:13 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 25 Feb 2021 04:16:13 GMT
VOLUME [/vault/logs]
# Thu, 25 Feb 2021 04:16:14 GMT
VOLUME [/vault/file]
# Thu, 25 Feb 2021 04:16:15 GMT
EXPOSE 8200
# Thu, 25 Feb 2021 04:16:15 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 25 Feb 2021 04:16:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 04:16:17 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:1287318d28f14b1b909b2cd8ff908cb037ec28d475bcdf70d1b14fdc0869650f`  
		Last Modified: Wed, 24 Feb 2021 20:40:42 GMT  
		Size: 2.7 MB (2720385 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d6bdcf98a8f33143f5380d0058503d12cc6756895d54dfc775a763b88c78dc8`  
		Last Modified: Thu, 25 Feb 2021 04:17:25 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d94001555867ee89de33f77cfee4e8addd014546bcfd60387cab94b4b2d87925`  
		Last Modified: Thu, 25 Feb 2021 04:17:35 GMT  
		Size: 49.2 MB (49194343 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d59dcfbce7fcf49406ad4b08a13dcf3ac7282b364a18a5cd4836e7a2939ca42b`  
		Last Modified: Thu, 25 Feb 2021 04:17:27 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:499619716c039e9345346edb8a71b33536d86ef5b173f95aa5e5c04ef6729bbf`  
		Last Modified: Thu, 25 Feb 2021 04:17:25 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.7` - linux; 386

```console
$ docker pull vault@sha256:2b9a146cb3edf59443b07c9901092aa9447db762cc4c6812a05556f4aeb8df29
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53087089 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:160aa0d3093f1bb269b73de17a736230fe9098cb77e6ffabb723dd2b6bf8cbf5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:57 GMT
ADD file:b5ef4a4abd9ccb894bdda7a5750878d13fbac4746c7b173c5dc88cf4846fc976 in / 
# Wed, 24 Feb 2021 20:38:57 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:21:32 GMT
ARG VAULT_VERSION=1.5.7
# Thu, 25 Feb 2021 02:21:33 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 25 Feb 2021 02:21:40 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 25 Feb 2021 02:21:41 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 25 Feb 2021 02:21:41 GMT
VOLUME [/vault/logs]
# Thu, 25 Feb 2021 02:21:41 GMT
VOLUME [/vault/file]
# Thu, 25 Feb 2021 02:21:42 GMT
EXPOSE 8200
# Thu, 25 Feb 2021 02:21:42 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 25 Feb 2021 02:21:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:21:43 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:9c18aa22aceabbea5b9c3d26c1e449591c02413fb34b574d9f73520f3fea602b`  
		Last Modified: Wed, 24 Feb 2021 20:39:36 GMT  
		Size: 2.8 MB (2788780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9240bb1b514f2b7f3e3efc49b5909c685a3670458a07d24f90336a58d93d97f`  
		Last Modified: Thu, 25 Feb 2021 02:22:33 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b86a4dc009f1af52e9dab22d96058e7f8df3ecf156b045864a7794bc8054376`  
		Last Modified: Thu, 25 Feb 2021 02:22:43 GMT  
		Size: 50.3 MB (50295073 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1554a93ff68d03e54b6f47b347e0ea67562086c6a3b7ae18e3a7fc97c13d263d`  
		Last Modified: Thu, 25 Feb 2021 02:22:36 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:80edd1e6ad27f1537e6e11ec372b34df9ca92a80feddd2940f1242a17b27c250`  
		Last Modified: Thu, 25 Feb 2021 02:22:33 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.6.3`

```console
$ docker pull vault@sha256:761a08153d5cdcf9d4f08a7a0340e0737b45dabfc2ef52e5a54ce975dff65f21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.6.3` - linux; amd64

```console
$ docker pull vault@sha256:8c988769b7857a76c572beb69f836867b6b1897099aaa2e85c1eed63f8cb19ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68982695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d2d40c91b671fbbc35b1e96066a6c1801ded5a272403262b6441e1f83b9dcf8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 22:38:32 GMT
ARG VAULT_VERSION=1.6.3
# Tue, 02 Mar 2021 22:38:33 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 02 Mar 2021 22:38:40 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 02 Mar 2021 22:38:41 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 02 Mar 2021 22:38:42 GMT
VOLUME [/vault/logs]
# Tue, 02 Mar 2021 22:38:42 GMT
VOLUME [/vault/file]
# Tue, 02 Mar 2021 22:38:42 GMT
EXPOSE 8200
# Tue, 02 Mar 2021 22:38:42 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Mar 2021 22:38:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 22:38:43 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65ad4abc0dcc95b11580214ff3d8b5e96a58cbb69186abd08bba0a7262f2bac`  
		Last Modified: Tue, 02 Mar 2021 22:39:07 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f1792f1f13c93b2699849dc68c2838cf35640f56ed9f9933aa291eb6b52a7d`  
		Last Modified: Tue, 02 Mar 2021 22:39:27 GMT  
		Size: 66.2 MB (66167831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147e2dd13b4d0ed6710c93f5ac1d2fced07d8ce6fcaab52b30395988728c10d6`  
		Last Modified: Tue, 02 Mar 2021 22:39:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ed46026a365b67a9f57649168adef9a033eee26b2f2170f2d4770f8487ab27`  
		Last Modified: Tue, 02 Mar 2021 22:39:07 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.3` - linux; arm variant v6

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

### `vault:1.6.3` - linux; arm64 variant v8

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

### `vault:1.6.3` - linux; 386

```console
$ docker pull vault@sha256:9c794fb76bcf526305399f2312b4f6e7c5178870c8e1c8c2b57f9433befb3935
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67032941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ce1bf01bd4b573cb7e2695b1b57a652ebffec1f83306ff91a0775f111e47f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 21:38:34 GMT
ADD file:eaee53da3c87749799de55809e4a5b526c56855332b961a85b1184c660f1d65b in / 
# Wed, 17 Feb 2021 21:38:35 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 22:55:03 GMT
ARG VAULT_VERSION=1.6.3
# Tue, 02 Mar 2021 22:55:04 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 02 Mar 2021 22:55:12 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 02 Mar 2021 22:55:13 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 02 Mar 2021 22:55:13 GMT
VOLUME [/vault/logs]
# Tue, 02 Mar 2021 22:55:13 GMT
VOLUME [/vault/file]
# Tue, 02 Mar 2021 22:55:13 GMT
EXPOSE 8200
# Tue, 02 Mar 2021 22:55:13 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Mar 2021 22:55:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 22:55:14 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:86205afa28f6bc624469015a543d16608258d2828411a92c662f4fdc6d276e18`  
		Last Modified: Wed, 17 Feb 2021 21:39:07 GMT  
		Size: 2.8 MB (2818177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfefd6a7fc6f96fa9e2b8a8915039def6c21294514f18e301dd25f46961ba35`  
		Last Modified: Tue, 02 Mar 2021 22:55:33 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e379536aca41700df07659b45e9de5ec32913e9b74b80265e81eaaecc16263`  
		Last Modified: Tue, 02 Mar 2021 22:55:44 GMT  
		Size: 64.2 MB (64211563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95c2a90b3060e98be4be38bcce3da5d32785a769ff39f5613e733655436ed83`  
		Last Modified: Tue, 02 Mar 2021 22:55:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca38fd949f08647d67542b02f8058b4309ff75d35bf6ac0e35b5ddecd3c2caef`  
		Last Modified: Tue, 02 Mar 2021 22:55:33 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.7.0-rc1`

```console
$ docker pull vault@sha256:9a458f973f82ddab01c9834729280d5522f02e827b824db387726aabb65715c4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; arm variant v6

### `vault:1.7.0-rc1` - linux; arm variant v6

```console
$ docker pull vault@sha256:3774e40967516f02b0e1e95c0d6d5b2a0f5d2c1fc1b1444d925b9324ef08c5d1
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66701202 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9a076fb7281763a43289d7998affb280220ace610d2111bd206b4cffd71dddf0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 20:49:32 GMT
ADD file:c04fbd3b039001c592cfa14f8388f8934ed4223ccf274dbb926e75039e172af4 in / 
# Wed, 17 Feb 2021 20:49:33 GMT
CMD ["/bin/sh"]
# Fri, 12 Mar 2021 21:06:53 GMT
ARG VAULT_VERSION=1.7.0-rc1
# Fri, 12 Mar 2021 21:06:55 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 12 Mar 2021 21:07:07 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 12 Mar 2021 21:07:10 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 12 Mar 2021 21:07:11 GMT
VOLUME [/vault/logs]
# Fri, 12 Mar 2021 21:07:11 GMT
VOLUME [/vault/file]
# Fri, 12 Mar 2021 21:07:12 GMT
EXPOSE 8200
# Fri, 12 Mar 2021 21:07:13 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 12 Mar 2021 21:07:13 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 12 Mar 2021 21:07:14 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:1353527ebe111f9bb1e271264a3c182e909e4b36463f80d7dbde1be0713eb892`  
		Last Modified: Wed, 17 Feb 2021 20:50:06 GMT  
		Size: 2.6 MB (2622039 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:da71943561a84c5a71b50584dce69c1fa92edeb892379413a3ca6aee79713b9f`  
		Last Modified: Fri, 12 Mar 2021 21:07:42 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5fd520100b4e569f3cc80cfa37639845a4acc36da813548a31e3d7e49b1f4a5d`  
		Last Modified: Fri, 12 Mar 2021 21:08:00 GMT  
		Size: 64.1 MB (64075893 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fb7976f00f5bc42016b9f92eb0d013b94a23414c0d0c735630b236efe68d961e`  
		Last Modified: Fri, 12 Mar 2021 21:07:42 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e4fd12f56f70b0f61bc421d11e7f15e4ae533e2783e397cca3dd0c1d60a1371e`  
		Last Modified: Fri, 12 Mar 2021 21:07:42 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:761a08153d5cdcf9d4f08a7a0340e0737b45dabfc2ef52e5a54ce975dff65f21
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:8c988769b7857a76c572beb69f836867b6b1897099aaa2e85c1eed63f8cb19ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68982695 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d2d40c91b671fbbc35b1e96066a6c1801ded5a272403262b6441e1f83b9dcf8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 21:19:54 GMT
ADD file:80bf8bd014071345b1c0364eeb0a5e48f3fb0d87f9c31cb990e57caa652b59b8 in / 
# Wed, 17 Feb 2021 21:19:54 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 22:38:32 GMT
ARG VAULT_VERSION=1.6.3
# Tue, 02 Mar 2021 22:38:33 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 02 Mar 2021 22:38:40 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 02 Mar 2021 22:38:41 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 02 Mar 2021 22:38:42 GMT
VOLUME [/vault/logs]
# Tue, 02 Mar 2021 22:38:42 GMT
VOLUME [/vault/file]
# Tue, 02 Mar 2021 22:38:42 GMT
EXPOSE 8200
# Tue, 02 Mar 2021 22:38:42 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Mar 2021 22:38:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 22:38:43 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:ba3557a56b150f9b813f9d02274d62914fd8fce120dd374d9ee17b87cf1d277d`  
		Last Modified: Wed, 17 Feb 2021 21:20:25 GMT  
		Size: 2.8 MB (2811657 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c65ad4abc0dcc95b11580214ff3d8b5e96a58cbb69186abd08bba0a7262f2bac`  
		Last Modified: Tue, 02 Mar 2021 22:39:07 GMT  
		Size: 1.2 KB (1230 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78f1792f1f13c93b2699849dc68c2838cf35640f56ed9f9933aa291eb6b52a7d`  
		Last Modified: Tue, 02 Mar 2021 22:39:27 GMT  
		Size: 66.2 MB (66167831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:147e2dd13b4d0ed6710c93f5ac1d2fced07d8ce6fcaab52b30395988728c10d6`  
		Last Modified: Tue, 02 Mar 2021 22:39:07 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9ed46026a365b67a9f57649168adef9a033eee26b2f2170f2d4770f8487ab27`  
		Last Modified: Tue, 02 Mar 2021 22:39:07 GMT  
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
$ docker pull vault@sha256:9c794fb76bcf526305399f2312b4f6e7c5178870c8e1c8c2b57f9433befb3935
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67032941 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9ce1bf01bd4b573cb7e2695b1b57a652ebffec1f83306ff91a0775f111e47f0`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 17 Feb 2021 21:38:34 GMT
ADD file:eaee53da3c87749799de55809e4a5b526c56855332b961a85b1184c660f1d65b in / 
# Wed, 17 Feb 2021 21:38:35 GMT
CMD ["/bin/sh"]
# Tue, 02 Mar 2021 22:55:03 GMT
ARG VAULT_VERSION=1.6.3
# Tue, 02 Mar 2021 22:55:04 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 02 Mar 2021 22:55:12 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 02 Mar 2021 22:55:13 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 02 Mar 2021 22:55:13 GMT
VOLUME [/vault/logs]
# Tue, 02 Mar 2021 22:55:13 GMT
VOLUME [/vault/file]
# Tue, 02 Mar 2021 22:55:13 GMT
EXPOSE 8200
# Tue, 02 Mar 2021 22:55:13 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 02 Mar 2021 22:55:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 02 Mar 2021 22:55:14 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:86205afa28f6bc624469015a543d16608258d2828411a92c662f4fdc6d276e18`  
		Last Modified: Wed, 17 Feb 2021 21:39:07 GMT  
		Size: 2.8 MB (2818177 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:abfefd6a7fc6f96fa9e2b8a8915039def6c21294514f18e301dd25f46961ba35`  
		Last Modified: Tue, 02 Mar 2021 22:55:33 GMT  
		Size: 1.2 KB (1227 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:48e379536aca41700df07659b45e9de5ec32913e9b74b80265e81eaaecc16263`  
		Last Modified: Tue, 02 Mar 2021 22:55:44 GMT  
		Size: 64.2 MB (64211563 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95c2a90b3060e98be4be38bcce3da5d32785a769ff39f5613e733655436ed83`  
		Last Modified: Tue, 02 Mar 2021 22:55:33 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca38fd949f08647d67542b02f8058b4309ff75d35bf6ac0e35b5ddecd3c2caef`  
		Last Modified: Tue, 02 Mar 2021 22:55:33 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
