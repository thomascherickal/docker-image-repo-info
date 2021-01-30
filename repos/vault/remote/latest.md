## `vault:latest`

```console
$ docker pull vault@sha256:72c64b9478c2309b3ae26c3c8c3618f6e6fea74e18a6e170ca9128396a99e6bc
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
$ docker pull vault@sha256:d7667c632a9f4aea4090f1c2340f3208c8ea181f84125a1f19090bbdaeed2218
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.6 MB (63642037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5758a038f53ebb562d9f93b45274c75cb747b8389ee0b043e71f09f9a5893a24`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 15:51:35 GMT
ADD file:ef75120295e25a8e67c5ef378df2cf4ce9f7b83b44709452fcaf247b54fabd16 in / 
# Thu, 23 Apr 2020 15:51:36 GMT
CMD ["/bin/sh"]
# Sat, 30 Jan 2021 01:54:10 GMT
ARG VAULT_VERSION=1.6.2
# Sat, 30 Jan 2021 01:54:11 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 30 Jan 2021 01:54:24 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 30 Jan 2021 01:54:26 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 30 Jan 2021 01:54:27 GMT
VOLUME [/vault/logs]
# Sat, 30 Jan 2021 01:54:27 GMT
VOLUME [/vault/file]
# Sat, 30 Jan 2021 01:54:28 GMT
EXPOSE 8200
# Sat, 30 Jan 2021 01:54:29 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 30 Jan 2021 01:54:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Jan 2021 01:54:30 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:e745d1dc1c9e0be26166278da7632765ca98fa1be8179a7cc440b3bdc5671860`  
		Last Modified: Thu, 23 Apr 2020 15:52:15 GMT  
		Size: 2.6 MB (2572512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b7b0bbadbc619a1f3b16c8876be48e151172e38384ae597bc9eafb1a5bca2fa`  
		Last Modified: Sat, 30 Jan 2021 01:55:11 GMT  
		Size: 1.3 KB (1292 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae8d70bfc8bdba014de55a2d41e7b9595ef80e06759a631d5fee946d864f0bb3`  
		Last Modified: Sat, 30 Jan 2021 01:55:27 GMT  
		Size: 61.1 MB (61066222 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:871451d2756a8635dd4f5cca953701710b1bfc1878f3ffb708a358246e717a5f`  
		Last Modified: Sat, 30 Jan 2021 01:55:11 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:510c47e57879419df53b5e6443d4b456019204a73ae45d2447a23a04fb49d84e`  
		Last Modified: Sat, 30 Jan 2021 01:55:11 GMT  
		Size: 1.8 KB (1823 bytes)  
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
$ docker pull vault@sha256:7b6758cc50f231d3e712cbd61ed534508251a77e36b5b94d9328e2cf2ea621bb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (66977310 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ab6ca541ae2da3a354a39ea7930707bd53b02b1a8f0a328e1cf9e837d336c252`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Apr 2020 21:16:11 GMT
ADD file:2e9fb162fdd20e7ac6e9edcb9e1ce9ece750f125c93824c5709a2800ae397f89 in / 
# Thu, 23 Apr 2020 21:16:11 GMT
CMD ["/bin/sh"]
# Sat, 30 Jan 2021 01:39:29 GMT
ARG VAULT_VERSION=1.6.2
# Sat, 30 Jan 2021 01:39:30 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 30 Jan 2021 01:39:38 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 30 Jan 2021 01:39:39 GMT
# ARGS: VAULT_VERSION=1.6.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 30 Jan 2021 01:39:39 GMT
VOLUME [/vault/logs]
# Sat, 30 Jan 2021 01:39:39 GMT
VOLUME [/vault/file]
# Sat, 30 Jan 2021 01:39:39 GMT
EXPOSE 8200
# Sat, 30 Jan 2021 01:39:39 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 30 Jan 2021 01:39:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 30 Jan 2021 01:39:40 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:294658c31053f36b08a64158e37d4fb84478e6fe8f4d5127c51a6334c8a3c36d`  
		Last Modified: Thu, 23 Apr 2020 21:16:37 GMT  
		Size: 2.8 MB (2787128 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a11ca99113386e8cd7843582ea2eeeb39a18c1ea7e78adea7804c2e09ecd3998`  
		Last Modified: Sat, 30 Jan 2021 01:40:10 GMT  
		Size: 1.3 KB (1264 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ac9f5376185385704aac2735439be667ccebe4b01dd6c7fdc36ce41d9a5d93f5`  
		Last Modified: Sat, 30 Jan 2021 01:40:20 GMT  
		Size: 64.2 MB (64186940 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f762adef11116d15fa78bdf99f067482cd4e0bc7f8edb999c1c9286b279dbe40`  
		Last Modified: Sat, 30 Jan 2021 01:40:09 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65ebf76726b574005c516756570acb3326603671c8c82319050708f84cf02e62`  
		Last Modified: Sat, 30 Jan 2021 01:40:09 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
