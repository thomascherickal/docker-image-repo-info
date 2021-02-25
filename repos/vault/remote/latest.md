## `vault:latest`

```console
$ docker pull vault@sha256:9c557f35cb5ec21aebafa33ae8ad3d32e657b950ee10696f9c5d25cd3d4b8db7
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:3891ca2e808582c37ff79c661ec9924ae062014de01c4c663a636967d994b646
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.9 MB (68949623 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64665835d5865560b564d53790462b462c0f41ab46f3231cc096ecb12eca0d1e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 01:05:21 GMT
ADD file:66a440394c2442570f1f060e25c86613cb2d88a8af0c71c5a4154b3570e9a805 in / 
# Fri, 24 Apr 2020 01:05:21 GMT
CMD ["/bin/sh"]
# Sat, 30 Jan 2021 02:32:55 GMT
ARG VAULT_VERSION=1.6.2
# Sat, 30 Jan 2021 02:32:56 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 30 Jan 2021 02:33:03 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 30 Jan 2021 02:33:04 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 30 Jan 2021 02:33:04 GMT
VOLUME [/vault/logs]
# Sat, 30 Jan 2021 02:33:04 GMT
VOLUME [/vault/file]
# Sat, 30 Jan 2021 02:33:04 GMT
EXPOSE 8200
# Sat, 30 Jan 2021 02:33:05 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 30 Jan 2021 02:33:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Jan 2021 02:33:05 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:21c83c5242199776c232920ddb58cfa2a46b17e42ed831ca9001c8dbc532d22d`  
		Last Modified: Fri, 24 Apr 2020 01:06:07 GMT  
		Size: 2.8 MB (2795580 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:67dfcdbc8a1ac2e6a91b72add2019a61090701d2296c9d93c692e0ea05bf8568`  
		Last Modified: Sat, 30 Jan 2021 02:33:32 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5dd4c26996b1bc521b486b20aec46d22d991358ca6365ea5646610c2e603f9f`  
		Last Modified: Sat, 30 Jan 2021 02:33:42 GMT  
		Size: 66.2 MB (66150803 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0b63ae1409e87ff85da01bdfad67a4e84e906999d6b56b066329ea50b8ffe5db`  
		Last Modified: Sat, 30 Jan 2021 02:33:32 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:028736f26ea0214c8751295ed6cf7206f9027bf91f593dda5f86b3af5836db61`  
		Last Modified: Sat, 30 Jan 2021 02:33:33 GMT  
		Size: 1.8 KB (1825 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:365d4f2b2c9c071f5d281a140339088c0bcea0564721c2ce1d883e78212faeb8
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63644476 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9cb2a69288286a05d90da8f4bf96e5694a4daa9bfca7dde532b9645812dd4ee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:50:55 GMT
ADD file:9e81f449863b2d114afc239efa445f3bed6ff45b123ea3aad271a5631ac4fa13 in / 
# Wed, 24 Feb 2021 20:50:56 GMT
CMD ["/bin/sh"]
# Wed, 24 Feb 2021 23:36:56 GMT
ARG VAULT_VERSION=1.6.2
# Wed, 24 Feb 2021 23:36:59 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 24 Feb 2021 23:37:11 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 24 Feb 2021 23:37:14 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 24 Feb 2021 23:37:14 GMT
VOLUME [/vault/logs]
# Wed, 24 Feb 2021 23:37:15 GMT
VOLUME [/vault/file]
# Wed, 24 Feb 2021 23:37:16 GMT
EXPOSE 8200
# Wed, 24 Feb 2021 23:37:16 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 24 Feb 2021 23:37:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 24 Feb 2021 23:37:18 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:615b6501bf7ed56706d638bf075665f504b2fee0bdebf905dcb8610bc9271fa4`  
		Last Modified: Wed, 24 Feb 2021 20:51:33 GMT  
		Size: 2.6 MB (2574559 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46a155eb2b4c3461bb9c2d4b3092615ea5cd7c79024ed3321f3bc085ab3faf4e`  
		Last Modified: Wed, 24 Feb 2021 23:38:37 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7401d26ee49a2312a785a1ae464b59b3dccd26cdfefab0df9a530b8d0c1d2c24`  
		Last Modified: Wed, 24 Feb 2021 23:38:52 GMT  
		Size: 61.1 MB (61066624 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0787200f38137064dae13bdf155b2dc3f0930b091e259776046f5bcb69b707d0`  
		Last Modified: Wed, 24 Feb 2021 23:38:37 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a4d90f641b5ac0a6a14b19d230c617828f817743d0208b17f57163dfdbc619a`  
		Last Modified: Wed, 24 Feb 2021 23:38:37 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:5d19dda73172eaf68f3f97351b8997d63fb81853025a6ec24af4045a2918c58e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (65003474 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8165c0e602824c7a50eb305e3b94f2cb291fff4955dae9c88ff320dd82046357`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 24 Apr 2020 00:14:52 GMT
ADD file:75529f7e83edb6d0457a3b8bbfe33d4e3a12f339c5ace517d0f52dbedd9a146b in / 
# Fri, 24 Apr 2020 00:14:53 GMT
CMD ["/bin/sh"]
# Sat, 30 Jan 2021 01:42:17 GMT
ARG VAULT_VERSION=1.6.2
# Sat, 30 Jan 2021 01:42:19 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 30 Jan 2021 01:42:27 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 30 Jan 2021 01:42:29 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 30 Jan 2021 01:42:30 GMT
VOLUME [/vault/logs]
# Sat, 30 Jan 2021 01:42:31 GMT
VOLUME [/vault/file]
# Sat, 30 Jan 2021 01:42:31 GMT
EXPOSE 8200
# Sat, 30 Jan 2021 01:42:32 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 30 Jan 2021 01:42:33 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Jan 2021 01:42:33 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b038bcb63e9c8905cc879c957302f686a9b43f24a18dcfc4186ab236ddf04cad`  
		Last Modified: Fri, 24 Apr 2020 00:15:54 GMT  
		Size: 2.7 MB (2718734 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31023140a16d939fd3316e5c013e735f5b2199ff4fd68d2ee3a8046626cd8825`  
		Last Modified: Sat, 30 Jan 2021 01:43:19 GMT  
		Size: 1.3 KB (1291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d95b0dcc3cd0d10ba19db1130df6fec8abe5abdeafbb6fb16e9e7634d3d1c08`  
		Last Modified: Sat, 30 Jan 2021 01:43:32 GMT  
		Size: 62.3 MB (62281439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8f111f51485939ae0297844d458175b5cd697e43042a289cf0fc11874abca00`  
		Last Modified: Sat, 30 Jan 2021 01:43:19 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:86c78851589d6695666800a4c5e2b12ad7d454e5819058701d71b6ae957ec368`  
		Last Modified: Sat, 30 Jan 2021 01:43:19 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:f65d8e13320cd4b57dad4f027b1ca7ad8189c7e5506361119b74e477ca789b92
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (66979396 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fdf41b24780052937fb07f3f159ad9e799c57f8ef2d2f89eabc9cc3e7f3c674c`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 24 Feb 2021 20:38:57 GMT
ADD file:b5ef4a4abd9ccb894bdda7a5750878d13fbac4746c7b173c5dc88cf4846fc976 in / 
# Wed, 24 Feb 2021 20:38:57 GMT
CMD ["/bin/sh"]
# Thu, 25 Feb 2021 02:21:16 GMT
ARG VAULT_VERSION=1.6.2
# Thu, 25 Feb 2021 02:21:17 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 25 Feb 2021 02:21:25 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 25 Feb 2021 02:21:26 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 25 Feb 2021 02:21:26 GMT
VOLUME [/vault/logs]
# Thu, 25 Feb 2021 02:21:26 GMT
VOLUME [/vault/file]
# Thu, 25 Feb 2021 02:21:26 GMT
EXPOSE 8200
# Thu, 25 Feb 2021 02:21:27 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 25 Feb 2021 02:21:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 25 Feb 2021 02:21:27 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:9c18aa22aceabbea5b9c3d26c1e449591c02413fb34b574d9f73520f3fea602b`  
		Last Modified: Wed, 24 Feb 2021 20:39:36 GMT  
		Size: 2.8 MB (2788780 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4b0fc52b079229357fc9195698dc4303c0e212ed15301e27bb83fd11eedbe9e2`  
		Last Modified: Thu, 25 Feb 2021 02:22:10 GMT  
		Size: 1.3 KB (1260 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2e63ce9a15940c0601a22101e5fd26d317785bcedbfe3109bdc8239cdc1c3bd8`  
		Last Modified: Thu, 25 Feb 2021 02:22:22 GMT  
		Size: 64.2 MB (64187381 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bdd573b73273525828bd1f2b8a0ee74247d3ff81a81e3e3ad7570cc66cd04373`  
		Last Modified: Thu, 25 Feb 2021 02:22:10 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:208e73e1767b2f4838dc4384ab6af198011b113124018ef666946a3dc1b3475f`  
		Last Modified: Thu, 25 Feb 2021 02:22:10 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
