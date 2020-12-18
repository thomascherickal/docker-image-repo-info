## `vault:latest`

```console
$ docker pull vault@sha256:efe6036315aafbab771939cf518943ef704f5e02a96a0e1b2643666a4aab1ad4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:e2fedbd8dadb71d909c7f989c8182b82052107aeb09f62ec18e5fb24fc622c53
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68874640 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a75c4d4ace1ce551f74af61697a051a1b5e33905a306139c48e69b6e5aa23ab5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Fri, 18 Dec 2020 07:10:00 GMT
ARG VAULT_VERSION=1.6.1
# Fri, 18 Dec 2020 07:10:01 GMT
# ARGS: VAULT_VERSION=1.6.1
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 18 Dec 2020 07:10:07 GMT
# ARGS: VAULT_VERSION=1.6.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 18 Dec 2020 07:10:08 GMT
# ARGS: VAULT_VERSION=1.6.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 18 Dec 2020 07:10:08 GMT
VOLUME [/vault/logs]
# Fri, 18 Dec 2020 07:10:08 GMT
VOLUME [/vault/file]
# Fri, 18 Dec 2020 07:10:09 GMT
EXPOSE 8200
# Fri, 18 Dec 2020 07:10:09 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Dec 2020 07:10:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Dec 2020 07:10:09 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2552eed26cd446794896194a8ba6771c175eb63af44dc892f43291e633b28e7e`  
		Last Modified: Fri, 18 Dec 2020 07:10:37 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6096191328ae03c73cd428f5d3dab04af6979031f9d65a7a070967445682a97`  
		Last Modified: Fri, 18 Dec 2020 07:10:47 GMT  
		Size: 66.1 MB (66075823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63cf312915ed5fbc9ebffea9eb7575981ad9cbb3e2b3c5c368a0958001b73993`  
		Last Modified: Fri, 18 Dec 2020 07:10:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba2ada45d14dbebb82e88374bff41382edf0874c00d4c1ceb629d0c31aed8e9a`  
		Last Modified: Fri, 18 Dec 2020 07:10:36 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:545cabdf54d23483a831465550e07a61729c2e355d456fa186072f88b4e8d1f9
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63609506 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:893298f4e95f8ea646d77182e222108abb7577f0ee8ddbab6513c5f1c7fa01f7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 22:55:43 GMT
ARG VAULT_VERSION=1.6.1
# Thu, 17 Dec 2020 22:55:46 GMT
# ARGS: VAULT_VERSION=1.6.1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 17 Dec 2020 22:56:03 GMT
# ARGS: VAULT_VERSION=1.6.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 17 Dec 2020 22:56:06 GMT
# ARGS: VAULT_VERSION=1.6.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 17 Dec 2020 22:56:07 GMT
VOLUME [/vault/logs]
# Thu, 17 Dec 2020 22:56:07 GMT
VOLUME [/vault/file]
# Thu, 17 Dec 2020 22:56:08 GMT
EXPOSE 8200
# Thu, 17 Dec 2020 22:56:08 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 22:56:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 22:56:10 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0598157047c3458e454b48453ec585c7766faa9030cc2b1a57815c06e5c581e`  
		Last Modified: Thu, 17 Dec 2020 22:56:55 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:926860bd44513d75eb7170d49f71f1c1802e99adafe195a2042f9174a6727529`  
		Last Modified: Thu, 17 Dec 2020 22:57:12 GMT  
		Size: 61.0 MB (61033691 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:721c6c1ceafc38528ffb2ea65a71fbb43b36452765d2ccd0ea1ab2f9b6a2dbe6`  
		Last Modified: Thu, 17 Dec 2020 22:56:56 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f601b70554af679f5fa90fb52d60ac72c9639b6e26a54c0303695f976f5f9f8`  
		Last Modified: Thu, 17 Dec 2020 22:56:55 GMT  
		Size: 1.8 KB (1826 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:0917d1ea32765692b67dd26bddd3b7a7e587dc827eb7af2cc72b727f8fe4bce6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64951682 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a60160733ff6e167f19d2e56af4605380862095acc3263dccb712bd96caf9ac8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Fri, 18 Dec 2020 18:41:16 GMT
ARG VAULT_VERSION=1.6.1
# Fri, 18 Dec 2020 18:41:17 GMT
# ARGS: VAULT_VERSION=1.6.1
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 18 Dec 2020 18:41:26 GMT
# ARGS: VAULT_VERSION=1.6.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 18 Dec 2020 18:41:28 GMT
# ARGS: VAULT_VERSION=1.6.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 18 Dec 2020 18:41:29 GMT
VOLUME [/vault/logs]
# Fri, 18 Dec 2020 18:41:29 GMT
VOLUME [/vault/file]
# Fri, 18 Dec 2020 18:41:30 GMT
EXPOSE 8200
# Fri, 18 Dec 2020 18:41:30 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 18 Dec 2020 18:41:31 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 18 Dec 2020 18:41:32 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f3c351339b90c2cd39d7737698fc958bc6e9c9a83d045d0ff693a8f02c87504`  
		Last Modified: Fri, 18 Dec 2020 18:42:11 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66497d036eb57049b232e2eb9f9805068d608f9eca859919b51620728839a940`  
		Last Modified: Fri, 18 Dec 2020 18:42:24 GMT  
		Size: 62.2 MB (62229647 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03894842047357f4eb4cf135391175648a6c4927cd0367fee33a10be77c956f9`  
		Last Modified: Fri, 18 Dec 2020 18:42:11 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:395bb15ae9a97dea4edd981c964896ff82644aab0c734cc2671fc73de36fe5d6`  
		Last Modified: Fri, 18 Dec 2020 18:42:10 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:d473db1696cb8247f264ce7a8808f2fb47d237d027bbee657eaaf3367d89246c
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66924057 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e1a6565722078f87690c8120b67d35f29b72223156082699af4782f133cee98f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Thu, 17 Dec 2020 23:40:46 GMT
ARG VAULT_VERSION=1.6.1
# Thu, 17 Dec 2020 23:40:48 GMT
# ARGS: VAULT_VERSION=1.6.1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 17 Dec 2020 23:41:02 GMT
# ARGS: VAULT_VERSION=1.6.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 17 Dec 2020 23:41:03 GMT
# ARGS: VAULT_VERSION=1.6.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 17 Dec 2020 23:41:04 GMT
VOLUME [/vault/logs]
# Thu, 17 Dec 2020 23:41:04 GMT
VOLUME [/vault/file]
# Thu, 17 Dec 2020 23:41:05 GMT
EXPOSE 8200
# Thu, 17 Dec 2020 23:41:05 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 17 Dec 2020 23:41:06 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 17 Dec 2020 23:41:06 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e398a466ddf29c83196cd216906c4347ad785e2132d82dc2d05bd11a37008531`  
		Last Modified: Thu, 17 Dec 2020 23:41:52 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f85551220900ba071ed3483187e083e5db668428248f184d4f1c73509dce0ba`  
		Last Modified: Thu, 17 Dec 2020 23:42:19 GMT  
		Size: 64.1 MB (64133688 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a7c0b2e1164bbe1e23141a6d7846b13c3a4e7731c465bbbd1ed8de7edae0564`  
		Last Modified: Thu, 17 Dec 2020 23:41:53 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0cf70e3a3bc9706d32aec003f18c163060472eb8513916094de5aaaec39f6ea7`  
		Last Modified: Thu, 17 Dec 2020 23:41:52 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
