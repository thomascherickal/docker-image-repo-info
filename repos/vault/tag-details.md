<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.3.3`](#vault133)
-	[`vault:1.4.0-beta1`](#vault140-beta1)
-	[`vault:latest`](#vaultlatest)

## `vault:1.3.3`

```console
$ docker pull vault@sha256:a8409dff6597f2ef5f7ecd3c672671bb2af9a390073efd74f95c54aa41cba22a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:

## `vault:1.4.0-beta1`

```console
$ docker pull vault@sha256:a54469a8c963d88f4dc86a8d66374cd4be294edc761fdeaf8a8df498960f8f79
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.4.0-beta1` - linux; amd64

```console
$ docker pull vault@sha256:f205e369306f6ec204c79f7ba69853eafaa1813e80302135c43184287de0cc3f
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (52010840 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:647def44c08ce03b2365e39336050bec86a690236a0d4f540709489e23fb5420`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 21 Feb 2020 21:26:28 GMT
ARG VAULT_VERSION=1.4.0-beta1
# Fri, 21 Feb 2020 21:26:29 GMT
# ARGS: VAULT_VERSION=1.4.0-beta1
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Feb 2020 21:26:34 GMT
# ARGS: VAULT_VERSION=1.4.0-beta1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Feb 2020 21:26:35 GMT
# ARGS: VAULT_VERSION=1.4.0-beta1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Feb 2020 21:26:35 GMT
VOLUME [/vault/logs]
# Fri, 21 Feb 2020 21:26:36 GMT
VOLUME [/vault/file]
# Fri, 21 Feb 2020 21:26:36 GMT
EXPOSE 8200
# Fri, 21 Feb 2020 21:26:36 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Feb 2020 21:26:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 21:26:36 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:272a4074827ee52e95a4e5079b43c16cc3391f6544f9fc3a8ad996e0bf2eb50d`  
		Last Modified: Fri, 21 Feb 2020 21:26:43 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a44c454a98d38abd880a52c4ca26fd9a864c1b33b88a01a8f320e96016b81884`  
		Last Modified: Fri, 21 Feb 2020 21:26:51 GMT  
		Size: 49.2 MB (49220640 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e4af8f08e0e6dc3678e7ff64d15bb9e3dfdf6bbcd01b62948fe0d53089535e`  
		Last Modified: Fri, 21 Feb 2020 21:26:44 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6ad56ffcb217e17583660bb2eedf0159c9276cfad7dbac7b3eea493ebd461d44`  
		Last Modified: Fri, 21 Feb 2020 21:26:43 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.0-beta1` - linux; arm variant v6

```console
$ docker pull vault@sha256:18f6a12d2e98dd72116d6657708f04b6de0197bff85a1628bd7d55a70587199d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48658441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e723d691a8a55622790829b97ca72ea469c4450a30b95a9f5ae132ef815e4150`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Fri, 21 Feb 2020 21:49:58 GMT
ARG VAULT_VERSION=1.4.0-beta1
# Fri, 21 Feb 2020 21:50:03 GMT
# ARGS: VAULT_VERSION=1.4.0-beta1
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Feb 2020 21:50:23 GMT
# ARGS: VAULT_VERSION=1.4.0-beta1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Feb 2020 21:50:28 GMT
# ARGS: VAULT_VERSION=1.4.0-beta1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Feb 2020 21:50:32 GMT
VOLUME [/vault/logs]
# Fri, 21 Feb 2020 21:50:34 GMT
VOLUME [/vault/file]
# Fri, 21 Feb 2020 21:50:36 GMT
EXPOSE 8200
# Fri, 21 Feb 2020 21:50:37 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Feb 2020 21:50:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 21:50:41 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe4b3c5a0f821cd2e448c4335120bf374dec0ffc344e25cb3a1753dc820f515a`  
		Last Modified: Fri, 21 Feb 2020 21:50:58 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c933e1f4a0a7e1dde178db3224659ccce765e07ec28f3b0343620d65a97e12df`  
		Last Modified: Fri, 21 Feb 2020 21:51:11 GMT  
		Size: 46.1 MB (46083734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a758bd0497e4a9a3065cb5034fc0fcf25b9cc88e030ed643ec1086858e2e776`  
		Last Modified: Fri, 21 Feb 2020 21:50:58 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2df2496b20fd685d3461085fe4614aa083ebee8c6271c8eb91177b57502f884b`  
		Last Modified: Fri, 21 Feb 2020 21:50:58 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.0-beta1` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:a4f140b27b07bea97db23755bf721d1e8852b8912006a815ff695a4e5ba5c396
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.9 MB (48939708 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a90ec7c616f8543a5149501364684c011f996645ad63fe8e544a6f9cc80309d5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Fri, 21 Feb 2020 21:52:55 GMT
ARG VAULT_VERSION=1.4.0-beta1
# Fri, 21 Feb 2020 21:53:01 GMT
# ARGS: VAULT_VERSION=1.4.0-beta1
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Feb 2020 21:53:16 GMT
# ARGS: VAULT_VERSION=1.4.0-beta1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Feb 2020 21:53:19 GMT
# ARGS: VAULT_VERSION=1.4.0-beta1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Feb 2020 21:53:20 GMT
VOLUME [/vault/logs]
# Fri, 21 Feb 2020 21:53:21 GMT
VOLUME [/vault/file]
# Fri, 21 Feb 2020 21:53:22 GMT
EXPOSE 8200
# Fri, 21 Feb 2020 21:53:22 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Feb 2020 21:53:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 21:53:24 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a37d82371099a6031464bb8a2bf89a814b0da7b4fa9a131d6c45fba91adcf2b4`  
		Last Modified: Fri, 21 Feb 2020 21:53:33 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f4c2945e999b033dd935d7673478dc23db1593e44070ec4ec1a410a9d619974c`  
		Last Modified: Fri, 21 Feb 2020 21:53:44 GMT  
		Size: 46.2 MB (46218673 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55948ae29a81c6ac408c065af96b15708df1114031093f0e047576293c7d1397`  
		Last Modified: Fri, 21 Feb 2020 21:53:33 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:74cd49d4d08fd638433ee8dd2acacaef94630b58769bc8b131a1c9119f23b1d2`  
		Last Modified: Fri, 21 Feb 2020 21:53:33 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.0-beta1` - linux; 386

```console
$ docker pull vault@sha256:7b4d860b673ff4ba22ceff5e20fd702160b06bf2eb947f1f71918d4571fc768d
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50165076 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49068e7843b652e8aa3a43547ed10393a652a1c5d9f20f5913fa10785c6f5bd3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 21 Feb 2020 21:40:42 GMT
ARG VAULT_VERSION=1.4.0-beta1
# Fri, 21 Feb 2020 21:40:43 GMT
# ARGS: VAULT_VERSION=1.4.0-beta1
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 21 Feb 2020 21:40:49 GMT
# ARGS: VAULT_VERSION=1.4.0-beta1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 21 Feb 2020 21:40:50 GMT
# ARGS: VAULT_VERSION=1.4.0-beta1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 21 Feb 2020 21:40:50 GMT
VOLUME [/vault/logs]
# Fri, 21 Feb 2020 21:40:50 GMT
VOLUME [/vault/file]
# Fri, 21 Feb 2020 21:40:50 GMT
EXPOSE 8200
# Fri, 21 Feb 2020 21:40:51 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 21 Feb 2020 21:40:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 21 Feb 2020 21:40:51 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05fe9d35f4094ce92e8ff3200455ad05b98eabd8a58190930016c0ca48c8c0df`  
		Last Modified: Fri, 21 Feb 2020 21:40:58 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c23873910db1a74fadc7d51e254613e4fdc8b692fe468e56938f4f88e6fcf0ab`  
		Last Modified: Fri, 21 Feb 2020 21:41:06 GMT  
		Size: 47.4 MB (47375981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:137e615ed509410ecf39f39850deb3adc26f3b85b958048951e0eaf337ed6ffd`  
		Last Modified: Fri, 21 Feb 2020 21:40:58 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7fa860f27f5af5474a9494573c478b199af71c0b491e275f0dafb9f7938d9fdc`  
		Last Modified: Fri, 21 Feb 2020 21:40:58 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:cf9d54f9a5ead66076066e208dbdca2094531036d4b053c596341cefb17ebf95
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:e6ed7d173e84765278879501b31ea7b475047f82a3b12e88aaf5640e8660f650
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51638279 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0542f65ae3d04bb12403061a9b15d63343c216b1752cfcad4fcc810e2a2d4d38`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 06:14:48 GMT
ARG VAULT_VERSION=1.3.2
# Fri, 24 Jan 2020 06:14:49 GMT
# ARGS: VAULT_VERSION=1.3.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 24 Jan 2020 06:14:58 GMT
# ARGS: VAULT_VERSION=1.3.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 24 Jan 2020 06:14:59 GMT
# ARGS: VAULT_VERSION=1.3.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 24 Jan 2020 06:14:59 GMT
VOLUME [/vault/logs]
# Fri, 24 Jan 2020 06:15:00 GMT
VOLUME [/vault/file]
# Fri, 24 Jan 2020 06:15:00 GMT
EXPOSE 8200
# Fri, 24 Jan 2020 06:15:00 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Jan 2020 06:15:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jan 2020 06:15:01 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a4e1345c4d7f4de6b1d2c870957f75d28e068e6d18f0a0b2f9e3593c79373738`  
		Last Modified: Fri, 24 Jan 2020 06:15:09 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bb275042a3c0194ea58eecab2f75cf1a48b99bcd0996a9c9c6738a411fefdc6`  
		Last Modified: Fri, 24 Jan 2020 06:15:23 GMT  
		Size: 48.8 MB (48848082 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d0eb2e7b022b3fe5a695cbdb6116e484029fac622abbc2094b54353da70dc88`  
		Last Modified: Fri, 24 Jan 2020 06:15:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23e88cf2315196aeba74ba0c6959311263c46069eb5380e2fe21364823626ac2`  
		Last Modified: Fri, 24 Jan 2020 06:15:09 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:ace471023cfc4737f5a82c2680bce7ec2983e027ec2c27db7b764120fa2453b7
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.6 MB (48648959 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:800c5f6c32e01ada90c16c5b1fd319c3b3b5c7bbcc601fe5f7a9871295a1b20c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 20:55:25 GMT
ARG VAULT_VERSION=1.3.2
# Thu, 23 Jan 2020 20:55:29 GMT
# ARGS: VAULT_VERSION=1.3.2
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 23 Jan 2020 20:55:40 GMT
# ARGS: VAULT_VERSION=1.3.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 23 Jan 2020 20:55:44 GMT
# ARGS: VAULT_VERSION=1.3.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 23 Jan 2020 20:55:44 GMT
VOLUME [/vault/logs]
# Thu, 23 Jan 2020 20:55:46 GMT
VOLUME [/vault/file]
# Thu, 23 Jan 2020 20:55:47 GMT
EXPOSE 8200
# Thu, 23 Jan 2020 20:55:48 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 20:55:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 20:55:51 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cb635609e19b305a9a1d8ee4b0596d2da091b38cd70bbee0a686547ce41c97ca`  
		Last Modified: Thu, 23 Jan 2020 20:56:03 GMT  
		Size: 1.3 KB (1287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:71eec7232ee57f98f7ba188234b448c8fab3791b8e92b29bfa00b72e49603523`  
		Last Modified: Thu, 23 Jan 2020 20:56:16 GMT  
		Size: 46.1 MB (46074256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:44f78ff3086e9bb54e05790bcf7d62a6b891dd911763c340890703b897ab7d42`  
		Last Modified: Thu, 23 Jan 2020 20:56:03 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1965bf3a3f6b1cd80ff3f7c0ff3c4e8881072ca3707d110ae32e0795f1142e0`  
		Last Modified: Thu, 23 Jan 2020 20:56:03 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:fb59ef841f6a2a6c17249c6c6022b7ae112a9304751e9b2993cb7de5709a0146
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48702901 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:eefedb0590727014f2974db2e71335bd117779fedfd9e503e44993d023d2131e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Thu, 23 Jan 2020 23:41:22 GMT
ARG VAULT_VERSION=1.3.2
# Thu, 23 Jan 2020 23:41:24 GMT
# ARGS: VAULT_VERSION=1.3.2
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 23 Jan 2020 23:41:33 GMT
# ARGS: VAULT_VERSION=1.3.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 23 Jan 2020 23:41:38 GMT
# ARGS: VAULT_VERSION=1.3.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 23 Jan 2020 23:41:39 GMT
VOLUME [/vault/logs]
# Thu, 23 Jan 2020 23:41:40 GMT
VOLUME [/vault/file]
# Thu, 23 Jan 2020 23:41:42 GMT
EXPOSE 8200
# Thu, 23 Jan 2020 23:41:42 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 23 Jan 2020 23:41:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 23 Jan 2020 23:41:44 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1830a2af380c9ff4b25756d94d9ae345955aea8b28fbc1106cade60b8f27b41d`  
		Last Modified: Thu, 23 Jan 2020 23:41:55 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51bdf02ed4c8e272e282b5359ad60ef433bd3c62a5e733d20d5cd5604df6f5c3`  
		Last Modified: Thu, 23 Jan 2020 23:42:13 GMT  
		Size: 46.0 MB (45981873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7607612f0494e36dba4135af80578f63abb54605226105b8135b46d859e9b83`  
		Last Modified: Thu, 23 Jan 2020 23:41:55 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:75922dd29f1883db8eb8da1cd47e5f2cb12ac2dfaf414208df09b84f79da7b35`  
		Last Modified: Thu, 23 Jan 2020 23:41:55 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:74e950bb4541160d4d7cb9200f004a50d91a578277583414b670db49f6b717d3
```

-	Docker Version: 18.06.1-ce
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50110877 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:14f26ccb3eb75275fd1b1e1855dabb0e07206b88e61bd754af988fdeb15a4051`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 24 Jan 2020 04:32:36 GMT
ARG VAULT_VERSION=1.3.2
# Fri, 24 Jan 2020 04:32:37 GMT
# ARGS: VAULT_VERSION=1.3.2
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 24 Jan 2020 04:32:43 GMT
# ARGS: VAULT_VERSION=1.3.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 24 Jan 2020 04:32:43 GMT
# ARGS: VAULT_VERSION=1.3.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 24 Jan 2020 04:32:44 GMT
VOLUME [/vault/logs]
# Fri, 24 Jan 2020 04:32:44 GMT
VOLUME [/vault/file]
# Fri, 24 Jan 2020 04:32:44 GMT
EXPOSE 8200
# Fri, 24 Jan 2020 04:32:44 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 24 Jan 2020 04:32:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 24 Jan 2020 04:32:45 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a27205cd8586f595eebce24e76df805e403ded7772a91a9b0c65ddf082f74abf`  
		Last Modified: Fri, 24 Jan 2020 04:32:53 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f971e76fdb90da2605e3de1f76341eba7911b1ca1dbe5187e2c252bbf76be04`  
		Last Modified: Fri, 24 Jan 2020 04:33:17 GMT  
		Size: 47.3 MB (47321783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7426136abf00fa06b929b6db8a6f3794dcac2ddde9a9b48a1c09c5d79f85a5c5`  
		Last Modified: Fri, 24 Jan 2020 04:32:52 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c581f6a392c05ea8a52de3c2de40aee374620bc6444909deac8c407f1b2adda0`  
		Last Modified: Fri, 24 Jan 2020 04:32:52 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
