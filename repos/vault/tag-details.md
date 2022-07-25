<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.10.5`](#vault1105)
-	[`vault:1.11.1`](#vault1111)
-	[`vault:1.8.12`](#vault1812)
-	[`vault:1.9.8`](#vault198)
-	[`vault:latest`](#vaultlatest)

## `vault:1.10.5`

```console
$ docker pull vault@sha256:2087acab63af6b4e8733f1c3222e567ae2351927a9f50ce3aacffe36dbbe0822
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.10.5` - linux; amd64

```console
$ docker pull vault@sha256:277d8d09d943bf055b736734023307d0546bc8053e7a124aee3e7b2a2f8558da
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **74.1 MB (74089793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f901e1166b2dd8db9f65deac03f54ad3e9a485bcc62501bb8fc3c6d4c9303128`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:18 GMT
ADD file:80b46be2fe86b402518b00758ff5d8556d92113dc267a002b6c72a5f9c6742a3 in / 
# Tue, 19 Jul 2022 22:20:18 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:26:31 GMT
ARG VAULT_VERSION=1.10.5
# Mon, 25 Jul 2022 18:26:31 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:26:39 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:26:40 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:26:40 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:26:40 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:26:40 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:26:40 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:26:40 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:26:41 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:decfdc335d9bae9ca06166e1a4fc2cdf8c2344a42d85c8a1d3f964aab59ecff5`  
		Last Modified: Tue, 19 Jul 2022 22:20:55 GMT  
		Size: 2.8 MB (2818512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b0d1506e2f97c6382e813adb751b731cf79fa5e8090b734f9338b6997f8b2446`  
		Last Modified: Mon, 25 Jul 2022 18:27:24 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dca36f123d2b4d658b90ed953fd8728513b65695ee0c677f7ed2cf81fe291b92`  
		Last Modified: Mon, 25 Jul 2022 18:27:33 GMT  
		Size: 71.3 MB (71268011 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:24612531c69e59f255ffd5d36d83f3dcb9ae9de98079395f828954a98d38dccb`  
		Last Modified: Mon, 25 Jul 2022 18:27:24 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d165de4fbd8da7ffa48a97a40dc23545a0f49c5df95e848cc8306630f983a99`  
		Last Modified: Mon, 25 Jul 2022 18:27:24 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.10.5` - linux; arm variant v6

```console
$ docker pull vault@sha256:1c90f0783bc00f968aa8211b2f8115ac77ac585148a2e7c1abe14af14e2e92a3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.4 MB (67356440 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:42f83015e7056fad5abcec26553cc1145b842448a39ef127817080a5d496c0b4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:50:02 GMT
ADD file:5a22b2130f6fbe534730df1f47715641a45e55845be7f35c3183e2b74ec43397 in / 
# Tue, 19 Jul 2022 22:50:03 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:54:58 GMT
ARG VAULT_VERSION=1.10.5
# Mon, 25 Jul 2022 18:54:59 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:55:18 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:55:20 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:55:21 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:55:21 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:55:22 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:55:22 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:55:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:55:23 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7dc1cbfb63ac7071e143ce96f0f140dc30282039f8d0770eaa7ab97eba515639`  
		Last Modified: Tue, 19 Jul 2022 22:51:41 GMT  
		Size: 2.6 MB (2626632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3cc897d1c19eaf64128b971cfb0b7aa09aa312275705766c6c5e815c803bd6b7`  
		Last Modified: Mon, 25 Jul 2022 18:57:26 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69cfbd7d94fff49fcdccc0ee4760587ba8b0ff42eeceeac11bf982faf82d3863`  
		Last Modified: Mon, 25 Jul 2022 18:57:59 GMT  
		Size: 64.7 MB (64726537 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:934d2d43adde006a14da468c8c76d566519551e8efd9acf7a6f2782d04a7e0df`  
		Last Modified: Mon, 25 Jul 2022 18:57:26 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:df66309decd1e3f61c5a20d6f6fc8dd37c2e7f14896a8ef2881cf0ee0024d3a3`  
		Last Modified: Mon, 25 Jul 2022 18:57:26 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.10.5` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:4ecb1ffa3f685473eaa5a782e898dc315cd885179570dad5228e0db93a0e22c3
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.1 MB (69132755 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4418711d73c85745d314136bbb0a731a206a56ce5edfdf5b8573df80b6a2f4dd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:51 GMT
ADD file:bb30934245445dabbe698387b5d454c2360d05055f7ab1bcaaffefea5aefb539 in / 
# Tue, 19 Jul 2022 22:39:51 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:47:19 GMT
ARG VAULT_VERSION=1.10.5
# Mon, 25 Jul 2022 18:47:20 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:47:27 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:47:27 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:47:28 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:47:29 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:47:30 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:47:32 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:47:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:47:33 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f4bf3852c6ccaad2dedd57347d310f084247a2e202c2fc20f5fa88d921e8510e`  
		Last Modified: Tue, 19 Jul 2022 22:40:44 GMT  
		Size: 2.7 MB (2717747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa3f17a8ac6bc03dd8068241227da9a24f5326bdccc96be920b779641bc3c4d1`  
		Last Modified: Mon, 25 Jul 2022 18:48:36 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:33cbac59670e650333995fb367b7687f003d19498aff5532a5b61808bcdededf`  
		Last Modified: Mon, 25 Jul 2022 18:48:45 GMT  
		Size: 66.4 MB (66411797 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6988409cc9551f18a05b17c72b7ead8d0104116934faf7fa0c8a0a8c4f6c954a`  
		Last Modified: Mon, 25 Jul 2022 18:48:36 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3057349c20837d5d7db797adf80aca4ef441d382abe2a0f84e7e678deb1d24e8`  
		Last Modified: Mon, 25 Jul 2022 18:48:36 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.10.5` - linux; 386

```console
$ docker pull vault@sha256:e02e4fbaf485c5806fcf6994f865f57fc13bed3aa948d7c4006d9f68b35eeeae
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.4 MB (70432867 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f44e60dc05930f3a305c085d330031d5ca853fbfd194601b08171a878276e6d3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:38:40 GMT
ADD file:4ae4391bf852a3e83cff6c0baebf0241d4955d580e24c180f882a142e4adaf1d in / 
# Tue, 19 Jul 2022 22:38:40 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:40:56 GMT
ARG VAULT_VERSION=1.10.5
# Mon, 25 Jul 2022 18:40:57 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:41:05 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:41:05 GMT
# ARGS: VAULT_VERSION=1.10.5
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:41:06 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:41:07 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:41:08 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:41:10 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:41:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:41:11 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:cbf9934fc184d27d98bef2567dbcecbee05767c8762c95e63984577a8c23e961`  
		Last Modified: Tue, 19 Jul 2022 22:39:35 GMT  
		Size: 2.8 MB (2821611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:162e2940d3a156aa231f7844b29540536335664b1f65405034a51dc20839c768`  
		Last Modified: Mon, 25 Jul 2022 18:42:14 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88a3fda200e0d7e71d149cea1c41cfd280fb71acc00d4ffd57d05efa30363e77`  
		Last Modified: Mon, 25 Jul 2022 18:42:22 GMT  
		Size: 67.6 MB (67608050 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b80f64f757c56ff2e6377ee7a7000f2564edf058d489ccd60374b792e39994c0`  
		Last Modified: Mon, 25 Jul 2022 18:42:14 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38651dd9878611bac2c31b8d5daee28584e6d32ec217cb268ab80f80e6e4be45`  
		Last Modified: Mon, 25 Jul 2022 18:42:14 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.11.1`

```console
$ docker pull vault@sha256:594d69ae0e3f7d8422a99859fd8221d8b558bb65ce561e433d2b25bdfb6d65bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.11.1` - linux; amd64

```console
$ docker pull vault@sha256:3431c4abf0626b6dcdc5e089b50f45f42b02e70c0e8e052dbfa7b286112b783c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.5 MB (77485808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:110083e80db2708862990fa140cc3d77f5d7e49e42b798b3c9430cd15ab36d23`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:18 GMT
ADD file:80b46be2fe86b402518b00758ff5d8556d92113dc267a002b6c72a5f9c6742a3 in / 
# Tue, 19 Jul 2022 22:20:18 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:26:17 GMT
ARG VAULT_VERSION=1.11.1
# Mon, 25 Jul 2022 18:26:18 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:26:25 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:26:26 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:26:26 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:26:27 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:26:27 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:26:27 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:26:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:26:27 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:decfdc335d9bae9ca06166e1a4fc2cdf8c2344a42d85c8a1d3f964aab59ecff5`  
		Last Modified: Tue, 19 Jul 2022 22:20:55 GMT  
		Size: 2.8 MB (2818512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca3ee0c4c0ee5120804e8b5fd08085d71d121c15aeba5e926f720c547e54b46`  
		Last Modified: Mon, 25 Jul 2022 18:27:05 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76510e381dd4cd2512d3c65f286f658f88a1b2bd0042a8cfe069a312cc2d317`  
		Last Modified: Mon, 25 Jul 2022 18:27:15 GMT  
		Size: 74.7 MB (74664027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2bd4372a720e0b04a197723fbd24f5136fc4b0c2de3be982054cbfebe79`  
		Last Modified: Mon, 25 Jul 2022 18:27:05 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec37abeb57a949d44480834bd221624fbca7cbd5719f0aa8062f13c01cb8dd3a`  
		Last Modified: Mon, 25 Jul 2022 18:27:05 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.11.1` - linux; arm variant v6

```console
$ docker pull vault@sha256:98c9126b162b9e1b4a76d528d5e23e8008d4efd24471b2a24e19f3235303c489
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70236940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:437883db4f8198c2e429a1a5b936c9d4731ffe73e386e5219708205f63d4bdeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:50:02 GMT
ADD file:5a22b2130f6fbe534730df1f47715641a45e55845be7f35c3183e2b74ec43397 in / 
# Tue, 19 Jul 2022 22:50:03 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:54:20 GMT
ARG VAULT_VERSION=1.11.1
# Mon, 25 Jul 2022 18:54:22 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:54:40 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:54:42 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:54:43 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:54:43 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:54:43 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:54:44 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:54:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:54:45 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7dc1cbfb63ac7071e143ce96f0f140dc30282039f8d0770eaa7ab97eba515639`  
		Last Modified: Tue, 19 Jul 2022 22:51:41 GMT  
		Size: 2.6 MB (2626632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64408bd5ab3d0e5e4773b74934893e04b7a08b0041b3ca4d11e841a25b2798c`  
		Last Modified: Mon, 25 Jul 2022 18:56:39 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0e97ab67f6449bfbc4d8387de9b207e2a31813ab12af4914111953a4a263c6`  
		Last Modified: Mon, 25 Jul 2022 18:57:15 GMT  
		Size: 67.6 MB (67607035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70887ade433f3491b63e747efaa5eacac8f771abff07a33b0f69859d1282388e`  
		Last Modified: Mon, 25 Jul 2022 18:56:39 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4d7402aa04c229a6a9adbb493644638ca155dc63e686bda38094e89cc61a6e`  
		Last Modified: Mon, 25 Jul 2022 18:56:39 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.11.1` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:23e64f3c8dcbac95cb2f712863d210c13989f17ada80d9695061a13485154f70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72279010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972c877a0587e7105921e0b6e26e63b4be80309aff951abcf57f7a29b5089cf1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:51 GMT
ADD file:bb30934245445dabbe698387b5d454c2360d05055f7ab1bcaaffefea5aefb539 in / 
# Tue, 19 Jul 2022 22:39:51 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:46:56 GMT
ARG VAULT_VERSION=1.11.1
# Mon, 25 Jul 2022 18:46:57 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:47:06 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:47:06 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:47:07 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:47:08 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:47:09 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:47:11 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:47:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:47:12 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f4bf3852c6ccaad2dedd57347d310f084247a2e202c2fc20f5fa88d921e8510e`  
		Last Modified: Tue, 19 Jul 2022 22:40:44 GMT  
		Size: 2.7 MB (2717747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238c5f568b61359cf138d0376616410d35fabee9a01a8bd5ebf7f32076a5ea1b`  
		Last Modified: Mon, 25 Jul 2022 18:48:17 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c2d9900f1e8bc2fe04ec635396a501bb731b1c931f8ba78f512eafbdf89257`  
		Last Modified: Mon, 25 Jul 2022 18:48:25 GMT  
		Size: 69.6 MB (69558053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793adf17781c41e5c31b1d57dfd46ff0adc23491aee35836a5348608a200fe79`  
		Last Modified: Mon, 25 Jul 2022 18:48:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7eb709fb9bdadf28af874b1c0517bd2ac8afe29ee29e2323a144b7bca2c4ab`  
		Last Modified: Mon, 25 Jul 2022 18:48:17 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.11.1` - linux; 386

```console
$ docker pull vault@sha256:8938d395ad12f3ffcfb9ea20c5464080a4e37117bbf2a392dfbed80d71a1962c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73548554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91410775fc7177d33e4563af19987a5af9a59a1b9f591a14afe3afb3cb50a15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:38:40 GMT
ADD file:4ae4391bf852a3e83cff6c0baebf0241d4955d580e24c180f882a142e4adaf1d in / 
# Tue, 19 Jul 2022 22:38:40 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:40:34 GMT
ARG VAULT_VERSION=1.11.1
# Mon, 25 Jul 2022 18:40:35 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:40:45 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:40:45 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:40:46 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:40:47 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:40:48 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:40:50 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:40:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:40:51 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:cbf9934fc184d27d98bef2567dbcecbee05767c8762c95e63984577a8c23e961`  
		Last Modified: Tue, 19 Jul 2022 22:39:35 GMT  
		Size: 2.8 MB (2821611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56983bae4db5d70483b1fc0e6fd191a35fb6c46ac28d150e898508e44b05f19`  
		Last Modified: Mon, 25 Jul 2022 18:41:55 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84562057087433d3a59ab1dfd2705434665e7dc80f8c4bc6ffe948bd9c8b42dc`  
		Last Modified: Mon, 25 Jul 2022 18:42:03 GMT  
		Size: 70.7 MB (70723739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20bf83133f8d12e9948a70f900fcf1bf3214db827d1848abcf3f693c37d50c2`  
		Last Modified: Mon, 25 Jul 2022 18:41:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca29bd6111720757140a909c280ae4f63e093b8436c817deea6363d48f907274`  
		Last Modified: Mon, 25 Jul 2022 18:41:55 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.8.12`

```console
$ docker pull vault@sha256:89811272ad5c3bbb36be75fe05ffad13a3957fadb66dee8add082b323977c2cb
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.8.12` - linux; amd64

```console
$ docker pull vault@sha256:f760660f16abe1798452e9a65f24764ab3d221842e585c9964750747d6666079
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70629338 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:957d5923bcda57d3479c7c7a59628034d45a1793c213b74aeac7d35a69303766`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:18 GMT
ADD file:80b46be2fe86b402518b00758ff5d8556d92113dc267a002b6c72a5f9c6742a3 in / 
# Tue, 19 Jul 2022 22:20:18 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 02:03:37 GMT
ARG VAULT_VERSION=1.8.12
# Wed, 20 Jul 2022 02:03:38 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 20 Jul 2022 02:03:45 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 20 Jul 2022 02:03:46 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 20 Jul 2022 02:03:46 GMT
VOLUME [/vault/logs]
# Wed, 20 Jul 2022 02:03:46 GMT
VOLUME [/vault/file]
# Wed, 20 Jul 2022 02:03:47 GMT
EXPOSE 8200
# Wed, 20 Jul 2022 02:03:47 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 20 Jul 2022 02:03:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 02:03:47 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:decfdc335d9bae9ca06166e1a4fc2cdf8c2344a42d85c8a1d3f964aab59ecff5`  
		Last Modified: Tue, 19 Jul 2022 22:20:55 GMT  
		Size: 2.8 MB (2818512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:764680553f286ca79045e8c7f9f2483ceb44654fe33ff10bc468e847be04d915`  
		Last Modified: Wed, 20 Jul 2022 02:04:49 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fea08665a6659cdbcc6a670501d66afb7e19381519017deb9f4a9a3236f6c632`  
		Last Modified: Wed, 20 Jul 2022 02:04:58 GMT  
		Size: 67.8 MB (67807558 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5abec44ce6906be260218571543938318bdf357c0a6f032c08b4ed020683d013`  
		Last Modified: Wed, 20 Jul 2022 02:04:49 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a1796437a6c9404a3aeb93ab7502b09ecdb74e5d8dae7af5192bd5ea7a25e225`  
		Last Modified: Wed, 20 Jul 2022 02:04:49 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.12` - linux; arm variant v6

```console
$ docker pull vault@sha256:c30a367d5e34ec68eb9b4f734d2413874c03680475c5fc09efc56e1d08496b13
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (64958096 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:294f6b9a2b80b1b2cf4b73276910a1bcd62dad21994277f4fc2652b8adc49ad4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:50:02 GMT
ADD file:5a22b2130f6fbe534730df1f47715641a45e55845be7f35c3183e2b74ec43397 in / 
# Tue, 19 Jul 2022 22:50:03 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 06:05:39 GMT
ARG VAULT_VERSION=1.8.12
# Wed, 20 Jul 2022 06:05:40 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 20 Jul 2022 06:05:55 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 20 Jul 2022 06:05:59 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 20 Jul 2022 06:06:00 GMT
VOLUME [/vault/logs]
# Wed, 20 Jul 2022 06:06:00 GMT
VOLUME [/vault/file]
# Wed, 20 Jul 2022 06:06:01 GMT
EXPOSE 8200
# Wed, 20 Jul 2022 06:06:02 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 20 Jul 2022 06:06:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 06:06:03 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7dc1cbfb63ac7071e143ce96f0f140dc30282039f8d0770eaa7ab97eba515639`  
		Last Modified: Tue, 19 Jul 2022 22:51:41 GMT  
		Size: 2.6 MB (2626632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3eff56e064b3c060c3542b6290cd86f704f49b5de661a6a571f355daf0a9d09c`  
		Last Modified: Wed, 20 Jul 2022 06:08:51 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7593905a9e8639af6080049e64016336b135cbca9f5880b16c096caed97c6355`  
		Last Modified: Wed, 20 Jul 2022 06:09:24 GMT  
		Size: 62.3 MB (62328196 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:464bdb37f05941ccaf653dc75453f6410a43f64d86191449e03129b438f0c2e6`  
		Last Modified: Wed, 20 Jul 2022 06:08:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2af264c08b7e096e050297de1e970f403e8447e9e4123f855bc71ef6c92fda23`  
		Last Modified: Wed, 20 Jul 2022 06:08:51 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.12` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:949fab7fb7e5e74dd7ba87f0d9b8d6f582d7ecbfa63550cf2dcc72684ce06365
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.9 MB (66894495 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2c33ec0af9ce73fce03331993cb0a4b29442d77cd215865d7b701fd11ddfb3ef`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:51 GMT
ADD file:bb30934245445dabbe698387b5d454c2360d05055f7ab1bcaaffefea5aefb539 in / 
# Tue, 19 Jul 2022 22:39:51 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 03:51:38 GMT
ARG VAULT_VERSION=1.8.12
# Wed, 20 Jul 2022 03:51:39 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 20 Jul 2022 03:51:46 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 20 Jul 2022 03:51:47 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 20 Jul 2022 03:51:48 GMT
VOLUME [/vault/logs]
# Wed, 20 Jul 2022 03:51:49 GMT
VOLUME [/vault/file]
# Wed, 20 Jul 2022 03:51:50 GMT
EXPOSE 8200
# Wed, 20 Jul 2022 03:51:52 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 20 Jul 2022 03:51:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 03:51:53 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f4bf3852c6ccaad2dedd57347d310f084247a2e202c2fc20f5fa88d921e8510e`  
		Last Modified: Tue, 19 Jul 2022 22:40:44 GMT  
		Size: 2.7 MB (2717747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae5739e7300a3f66f5f739195564c911c9993c36c3b4f324135a61c92283e68d`  
		Last Modified: Wed, 20 Jul 2022 03:53:04 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:292ee0d66eeb81c4100ff44e627e07789f0ceb8957d5973a8972b27afc4ed85b`  
		Last Modified: Wed, 20 Jul 2022 03:53:13 GMT  
		Size: 64.2 MB (64173545 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b075f1388274672299fa3c442ac428883b29b402787c9787d6c6937966b1887`  
		Last Modified: Wed, 20 Jul 2022 03:53:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09037a42f58c1807755b846e6c1709cd3ab8a9cda3938d1c081b4d7c8ab8c01c`  
		Last Modified: Wed, 20 Jul 2022 03:53:05 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.8.12` - linux; 386

```console
$ docker pull vault@sha256:32ebaf7e4529bfe81aeedaa8216c99a19669562da53b4b1204f11d031c560360
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68326802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21fc5a803a9a87bdb00bc441ec078c9547dd4e3cb04d89d3783fbd8e918db0b5`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:38:40 GMT
ADD file:4ae4391bf852a3e83cff6c0baebf0241d4955d580e24c180f882a142e4adaf1d in / 
# Tue, 19 Jul 2022 22:38:40 GMT
CMD ["/bin/sh"]
# Wed, 20 Jul 2022 02:29:36 GMT
ARG VAULT_VERSION=1.8.12
# Wed, 20 Jul 2022 02:29:37 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 20 Jul 2022 02:29:46 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 20 Jul 2022 02:29:46 GMT
# ARGS: VAULT_VERSION=1.8.12
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 20 Jul 2022 02:29:47 GMT
VOLUME [/vault/logs]
# Wed, 20 Jul 2022 02:29:48 GMT
VOLUME [/vault/file]
# Wed, 20 Jul 2022 02:29:49 GMT
EXPOSE 8200
# Wed, 20 Jul 2022 02:29:51 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 20 Jul 2022 02:29:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 20 Jul 2022 02:29:52 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:cbf9934fc184d27d98bef2567dbcecbee05767c8762c95e63984577a8c23e961`  
		Last Modified: Tue, 19 Jul 2022 22:39:35 GMT  
		Size: 2.8 MB (2821611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e49728480c9e7419ec19690d2aa5b56574e1322ba5d41e26c470f89aa75ee5b`  
		Last Modified: Wed, 20 Jul 2022 02:31:04 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b7624d2c9bbf9e52e3e90d53e674a621327d42ac4bfd7c084c8fd09d8573240f`  
		Last Modified: Wed, 20 Jul 2022 02:31:14 GMT  
		Size: 65.5 MB (65501989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:809ecc92ae4da1a4298fb8657ea292248d8c835f2f82bfd8ad0653fd6b8f7232`  
		Last Modified: Wed, 20 Jul 2022 02:31:04 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92b8b5dc478893db3d6e132d54ffe7186a24dc97a4147b2c2a863c66de57f81f`  
		Last Modified: Wed, 20 Jul 2022 02:31:04 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.9.8`

```console
$ docker pull vault@sha256:9f5f4e9169c4a4af2e2c0c27ec561b863548f78fa5e676a3d668d1ad30ff2c57
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.9.8` - linux; amd64

```console
$ docker pull vault@sha256:593a5364dff0dafcdb101d0bd8092875e5acbae517e231bc32b5b3481ecec616
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73199603 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ecedcd28664d2162538acaad15c33c55e2bd91ec10b0355e13defba9465d03a6`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:18 GMT
ADD file:80b46be2fe86b402518b00758ff5d8556d92113dc267a002b6c72a5f9c6742a3 in / 
# Tue, 19 Jul 2022 22:20:18 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:26:43 GMT
ARG VAULT_VERSION=1.9.8
# Mon, 25 Jul 2022 18:26:43 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:26:51 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:26:51 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:26:52 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:26:52 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:26:52 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:26:52 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:26:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:26:52 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:decfdc335d9bae9ca06166e1a4fc2cdf8c2344a42d85c8a1d3f964aab59ecff5`  
		Last Modified: Tue, 19 Jul 2022 22:20:55 GMT  
		Size: 2.8 MB (2818512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6b5a0cd1ec2a41c0b649bc8acea241e5e0cb3a952ca2935bf58d85bf3747b34`  
		Last Modified: Mon, 25 Jul 2022 18:27:40 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e74e5b92bef60e041eee83e865923e06a118a9c927845808c9ddb20351a82e94`  
		Last Modified: Mon, 25 Jul 2022 18:27:49 GMT  
		Size: 70.4 MB (70377824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c0128247a657b7f3fd1f5b939d551e4447c195160dba9dbe9369e60415af4813`  
		Last Modified: Mon, 25 Jul 2022 18:27:40 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebff7dfe8e9b394be2bc576d1706f486c389a578d3406526f7ea2e14b49cc511`  
		Last Modified: Mon, 25 Jul 2022 18:27:41 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.8` - linux; arm variant v6

```console
$ docker pull vault@sha256:c3625ba61980ef60adbcbd5b809463fb46b191c1a9118969c0b423ee8c8df168
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66519770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5193250cc72de07d0875c60b001d788349a0e664ea5181d7dd53b1f080314ea1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:50:02 GMT
ADD file:5a22b2130f6fbe534730df1f47715641a45e55845be7f35c3183e2b74ec43397 in / 
# Tue, 19 Jul 2022 22:50:03 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:55:35 GMT
ARG VAULT_VERSION=1.9.8
# Mon, 25 Jul 2022 18:55:37 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:55:53 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:55:55 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:55:56 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:55:56 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:55:57 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:55:57 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:55:57 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:55:58 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7dc1cbfb63ac7071e143ce96f0f140dc30282039f8d0770eaa7ab97eba515639`  
		Last Modified: Tue, 19 Jul 2022 22:51:41 GMT  
		Size: 2.6 MB (2626632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d1e69a33ea60d4d3acd868c88cf05dbde6f1818a99d0f245f95cfe67138503f1`  
		Last Modified: Mon, 25 Jul 2022 18:58:07 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a51ea62b84bb779d7941702ae80f4bc4969ef5d7d7a218e73220d96c469cb2b`  
		Last Modified: Mon, 25 Jul 2022 18:58:42 GMT  
		Size: 63.9 MB (63889869 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5609274e815922ab53a36752fd17cfe077a5517bcf45fe529d771aafd46d467`  
		Last Modified: Mon, 25 Jul 2022 18:58:07 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a7258d37e034627c3ac16c1de8827037a08698a52d5d135fbfec661f50b6a412`  
		Last Modified: Mon, 25 Jul 2022 18:58:07 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.8` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:adbdebeedb5dd1b435af34f4f0560ec36c1daaeafa02abbe80e9352f28515e87
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68298600 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3f8ffe037f74d5474787e312d476a9ce091e6c4428df18383ec521295f43e028`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:51 GMT
ADD file:bb30934245445dabbe698387b5d454c2360d05055f7ab1bcaaffefea5aefb539 in / 
# Tue, 19 Jul 2022 22:39:51 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:47:38 GMT
ARG VAULT_VERSION=1.9.8
# Mon, 25 Jul 2022 18:47:39 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:47:47 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:47:47 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:47:48 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:47:49 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:47:50 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:47:52 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:47:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:47:53 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f4bf3852c6ccaad2dedd57347d310f084247a2e202c2fc20f5fa88d921e8510e`  
		Last Modified: Tue, 19 Jul 2022 22:40:44 GMT  
		Size: 2.7 MB (2717747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:821dde4ee72be0b3dce89d78270d36d363ea3cdc77bc7ae57b09a8c9fc0a8f6a`  
		Last Modified: Mon, 25 Jul 2022 18:48:52 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927bf878fbb2620959ceff5dac81019cb574ee6ca40f63cdba5f11a0821d3723`  
		Last Modified: Mon, 25 Jul 2022 18:49:01 GMT  
		Size: 65.6 MB (65577649 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d3132cc1cfdff804bd1e1ca50e1311426d2d0903ba08f3185a1ef78e077aba05`  
		Last Modified: Mon, 25 Jul 2022 18:48:52 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebb03e7a5f0bd90fa24e41e353edf9b3857fa8927f41cc652f9d24705deaab2e`  
		Last Modified: Mon, 25 Jul 2022 18:48:52 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.8` - linux; 386

```console
$ docker pull vault@sha256:13d830b4b6397e14d107f0981c1cc3c495031fbd74c375db91031baad7e48809
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69562904 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31d79a859edc6629e2b371472a976a23e53059161a64d47aa87d81f3dff94ade`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:38:40 GMT
ADD file:4ae4391bf852a3e83cff6c0baebf0241d4955d580e24c180f882a142e4adaf1d in / 
# Tue, 19 Jul 2022 22:38:40 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:41:16 GMT
ARG VAULT_VERSION=1.9.8
# Mon, 25 Jul 2022 18:41:17 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:41:25 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:41:25 GMT
# ARGS: VAULT_VERSION=1.9.8
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:41:26 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:41:27 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:41:28 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:41:30 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:41:30 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:41:31 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:cbf9934fc184d27d98bef2567dbcecbee05767c8762c95e63984577a8c23e961`  
		Last Modified: Tue, 19 Jul 2022 22:39:35 GMT  
		Size: 2.8 MB (2821611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f11d72f58dc90a884daaeec26ca3039ebae1abc7dfa194718027366a2d442327`  
		Last Modified: Mon, 25 Jul 2022 18:42:30 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2626a9c667fea015edfab5183815851294d64595ed1557aaaa15b03641bb468`  
		Last Modified: Mon, 25 Jul 2022 18:42:37 GMT  
		Size: 66.7 MB (66738085 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:83b60ab4585b137a98aa60df68fb3bfd1d0ad783116fa36f325b03b7349656e9`  
		Last Modified: Mon, 25 Jul 2022 18:42:30 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d9f3fbc8a91292b394ff536f6ae4f93e6eb41c86344340bee5c80c72cef0718d`  
		Last Modified: Mon, 25 Jul 2022 18:42:30 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:594d69ae0e3f7d8422a99859fd8221d8b558bb65ce561e433d2b25bdfb6d65bd
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:3431c4abf0626b6dcdc5e089b50f45f42b02e70c0e8e052dbfa7b286112b783c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.5 MB (77485808 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:110083e80db2708862990fa140cc3d77f5d7e49e42b798b3c9430cd15ab36d23`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:20:18 GMT
ADD file:80b46be2fe86b402518b00758ff5d8556d92113dc267a002b6c72a5f9c6742a3 in / 
# Tue, 19 Jul 2022 22:20:18 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:26:17 GMT
ARG VAULT_VERSION=1.11.1
# Mon, 25 Jul 2022 18:26:18 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:26:25 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:26:26 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:26:26 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:26:27 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:26:27 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:26:27 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:26:27 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:26:27 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:decfdc335d9bae9ca06166e1a4fc2cdf8c2344a42d85c8a1d3f964aab59ecff5`  
		Last Modified: Tue, 19 Jul 2022 22:20:55 GMT  
		Size: 2.8 MB (2818512 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ca3ee0c4c0ee5120804e8b5fd08085d71d121c15aeba5e926f720c547e54b46`  
		Last Modified: Mon, 25 Jul 2022 18:27:05 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c76510e381dd4cd2512d3c65f286f658f88a1b2bd0042a8cfe069a312cc2d317`  
		Last Modified: Mon, 25 Jul 2022 18:27:15 GMT  
		Size: 74.7 MB (74664027 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1eb5d2bd4372a720e0b04a197723fbd24f5136fc4b0c2de3be982054cbfebe79`  
		Last Modified: Mon, 25 Jul 2022 18:27:05 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec37abeb57a949d44480834bd221624fbca7cbd5719f0aa8062f13c01cb8dd3a`  
		Last Modified: Mon, 25 Jul 2022 18:27:05 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:98c9126b162b9e1b4a76d528d5e23e8008d4efd24471b2a24e19f3235303c489
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70236940 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:437883db4f8198c2e429a1a5b936c9d4731ffe73e386e5219708205f63d4bdeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:50:02 GMT
ADD file:5a22b2130f6fbe534730df1f47715641a45e55845be7f35c3183e2b74ec43397 in / 
# Tue, 19 Jul 2022 22:50:03 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:54:20 GMT
ARG VAULT_VERSION=1.11.1
# Mon, 25 Jul 2022 18:54:22 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:54:40 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:54:42 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:54:43 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:54:43 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:54:43 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:54:44 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:54:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:54:45 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7dc1cbfb63ac7071e143ce96f0f140dc30282039f8d0770eaa7ab97eba515639`  
		Last Modified: Tue, 19 Jul 2022 22:51:41 GMT  
		Size: 2.6 MB (2626632 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c64408bd5ab3d0e5e4773b74934893e04b7a08b0041b3ca4d11e841a25b2798c`  
		Last Modified: Mon, 25 Jul 2022 18:56:39 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e0e97ab67f6449bfbc4d8387de9b207e2a31813ab12af4914111953a4a263c6`  
		Last Modified: Mon, 25 Jul 2022 18:57:15 GMT  
		Size: 67.6 MB (67607035 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70887ade433f3491b63e747efaa5eacac8f771abff07a33b0f69859d1282388e`  
		Last Modified: Mon, 25 Jul 2022 18:56:39 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0a4d7402aa04c229a6a9adbb493644638ca155dc63e686bda38094e89cc61a6e`  
		Last Modified: Mon, 25 Jul 2022 18:56:39 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:23e64f3c8dcbac95cb2f712863d210c13989f17ada80d9695061a13485154f70
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72279010 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:972c877a0587e7105921e0b6e26e63b4be80309aff951abcf57f7a29b5089cf1`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:39:51 GMT
ADD file:bb30934245445dabbe698387b5d454c2360d05055f7ab1bcaaffefea5aefb539 in / 
# Tue, 19 Jul 2022 22:39:51 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:46:56 GMT
ARG VAULT_VERSION=1.11.1
# Mon, 25 Jul 2022 18:46:57 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:47:06 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:47:06 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:47:07 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:47:08 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:47:09 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:47:11 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:47:11 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:47:12 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f4bf3852c6ccaad2dedd57347d310f084247a2e202c2fc20f5fa88d921e8510e`  
		Last Modified: Tue, 19 Jul 2022 22:40:44 GMT  
		Size: 2.7 MB (2717747 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:238c5f568b61359cf138d0376616410d35fabee9a01a8bd5ebf7f32076a5ea1b`  
		Last Modified: Mon, 25 Jul 2022 18:48:17 GMT  
		Size: 1.2 KB (1238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60c2d9900f1e8bc2fe04ec635396a501bb731b1c931f8ba78f512eafbdf89257`  
		Last Modified: Mon, 25 Jul 2022 18:48:25 GMT  
		Size: 69.6 MB (69558053 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:793adf17781c41e5c31b1d57dfd46ff0adc23491aee35836a5348608a200fe79`  
		Last Modified: Mon, 25 Jul 2022 18:48:17 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be7eb709fb9bdadf28af874b1c0517bd2ac8afe29ee29e2323a144b7bca2c4ab`  
		Last Modified: Mon, 25 Jul 2022 18:48:17 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:8938d395ad12f3ffcfb9ea20c5464080a4e37117bbf2a392dfbed80d71a1962c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73548554 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:91410775fc7177d33e4563af19987a5af9a59a1b9f591a14afe3afb3cb50a15a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 19 Jul 2022 22:38:40 GMT
ADD file:4ae4391bf852a3e83cff6c0baebf0241d4955d580e24c180f882a142e4adaf1d in / 
# Tue, 19 Jul 2022 22:38:40 GMT
CMD ["/bin/sh"]
# Mon, 25 Jul 2022 18:40:34 GMT
ARG VAULT_VERSION=1.11.1
# Mon, 25 Jul 2022 18:40:35 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN addgroup vault &&     adduser -S -G vault vault
# Mon, 25 Jul 2022 18:40:45 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Mon, 25 Jul 2022 18:40:45 GMT
# ARGS: VAULT_VERSION=1.11.1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Mon, 25 Jul 2022 18:40:46 GMT
VOLUME [/vault/logs]
# Mon, 25 Jul 2022 18:40:47 GMT
VOLUME [/vault/file]
# Mon, 25 Jul 2022 18:40:48 GMT
EXPOSE 8200
# Mon, 25 Jul 2022 18:40:50 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Mon, 25 Jul 2022 18:40:50 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Mon, 25 Jul 2022 18:40:51 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:cbf9934fc184d27d98bef2567dbcecbee05767c8762c95e63984577a8c23e961`  
		Last Modified: Tue, 19 Jul 2022 22:39:35 GMT  
		Size: 2.8 MB (2821611 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b56983bae4db5d70483b1fc0e6fd191a35fb6c46ac28d150e898508e44b05f19`  
		Last Modified: Mon, 25 Jul 2022 18:41:55 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:84562057087433d3a59ab1dfd2705434665e7dc80f8c4bc6ffe948bd9c8b42dc`  
		Last Modified: Mon, 25 Jul 2022 18:42:03 GMT  
		Size: 70.7 MB (70723739 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f20bf83133f8d12e9948a70f900fcf1bf3214db827d1848abcf3f693c37d50c2`  
		Last Modified: Mon, 25 Jul 2022 18:41:55 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca29bd6111720757140a909c280ae4f63e093b8436c817deea6363d48f907274`  
		Last Modified: Mon, 25 Jul 2022 18:41:55 GMT  
		Size: 1.8 KB (1809 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
