<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.10.10`](#vault11010)
-	[`vault:1.11.7`](#vault1117)
-	[`vault:1.12.3`](#vault1123)
-	[`vault:1.9.10`](#vault1910)
-	[`vault:latest`](#vaultlatest)

## `vault:1.10.10`

```console
$ docker pull vault@sha256:0375c7fe7a4dc9510aea3cc7ad24be5865f891852d8d734c419e96335a3ce4d0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.10.10` - linux; amd64

```console
$ docker pull vault@sha256:9fb60c017105167fff213fb5613b37e25d1570263d2aad100d5d0771915d6c4b
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **85.3 MB (85325092 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7a322f0eaf37a5b325b4ada20aa4fea02b14c1e2f4931b153e8b6e718e1f2fde`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:14:13 GMT
ARG VAULT_VERSION=1.10.10
# Sat, 11 Feb 2023 14:14:14 GMT
# ARGS: VAULT_VERSION=1.10.10
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 14:14:21 GMT
# ARGS: VAULT_VERSION=1.10.10
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 14:14:22 GMT
# ARGS: VAULT_VERSION=1.10.10
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 14:14:22 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 14:14:23 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 14:14:23 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 14:14:23 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 14:14:23 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:14:23 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:931c88f0c8d9a3d6b617fd0b7a71e5123be0da9aa9193afa1b2792f1522aadbe`  
		Last Modified: Sat, 11 Feb 2023 14:15:21 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e82b10dcdbbbf5077ed78c8f2246a80be56dc7082115e661a25721a0b095980`  
		Last Modified: Sat, 11 Feb 2023 14:15:30 GMT  
		Size: 82.5 MB (82492191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:380b115981ef20a208ca299c496a4303623c69f2526551807335cfbd5faa16a1`  
		Last Modified: Sat, 11 Feb 2023 14:15:21 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ca19b8a923fed4e15231af99b4a447e0ec42bc0219d365881c90ddbc1b5e3eb6`  
		Last Modified: Sat, 11 Feb 2023 14:15:21 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.10.10` - linux; arm variant v6

```console
$ docker pull vault@sha256:a86b1c207f43e5c9f1e2967bf69a73f26be9f857e8f682dfb28c1a5893fee741
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80423704 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ed7f06f408cdc59a89cb1fcdf252ddcdd33488197e88007aceb8686dd213f9e8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:41 GMT
ADD file:767f6566ea2c075838c0a86ca644a37e446f309f68952f5f921970f046abd252 in / 
# Fri, 10 Feb 2023 20:49:41 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:35:51 GMT
ARG VAULT_VERSION=1.10.10
# Sat, 11 Feb 2023 03:35:52 GMT
# ARGS: VAULT_VERSION=1.10.10
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 03:36:01 GMT
# ARGS: VAULT_VERSION=1.10.10
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 03:36:02 GMT
# ARGS: VAULT_VERSION=1.10.10
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 03:36:02 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 03:36:02 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 03:36:02 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 03:36:02 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 03:36:02 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 03:36:03 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7616dd32f4bf5fddffb2543afaac2355a5fc495348c01060cd67181e36343e96`  
		Last Modified: Fri, 10 Feb 2023 20:51:02 GMT  
		Size: 2.6 MB (2638152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee19e66c8ed85332fefa4d0458b1910d5f050a12a702101f23285f99c6dfb9cb`  
		Last Modified: Sat, 11 Feb 2023 03:37:21 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de8a3f597c725b6b0dfae42da0701ce1934b711db19d3952f46e2dc51d4ba6bc`  
		Last Modified: Sat, 11 Feb 2023 03:37:35 GMT  
		Size: 77.8 MB (77782345 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e2e7233a15534b9f5455d45dadc11fbd411cb0690909bf229b7b4841d38c754a`  
		Last Modified: Sat, 11 Feb 2023 03:37:21 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0e50641f0ba13afbee9deeade59ca2590f911c021c1454a8620a971e54a901c`  
		Last Modified: Sat, 11 Feb 2023 03:37:21 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.10.10` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:6de262b9f7145d647d5c734567f90a9840510c13490e314d6df44368d4cacc8e
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.4 MB (80422171 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9372735a32881b1a687ea94fbc38e33d948ef1c464059f4cb328db8a5cb263f4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:19 GMT
ADD file:50a841463966858f1c3ca87143cf96145d1d52f7349ef516adfbf21cdd5684fe in / 
# Fri, 10 Feb 2023 21:24:19 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:42:01 GMT
ARG VAULT_VERSION=1.10.10
# Sat, 11 Feb 2023 05:42:02 GMT
# ARGS: VAULT_VERSION=1.10.10
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 05:42:10 GMT
# ARGS: VAULT_VERSION=1.10.10
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 05:42:11 GMT
# ARGS: VAULT_VERSION=1.10.10
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 05:42:11 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 05:42:11 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 05:42:12 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 05:42:12 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 05:42:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:42:12 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:6f0e733d82e26042c603e231c39b56abbabdad66673a736ec71c69c65be95f41`  
		Last Modified: Fri, 10 Feb 2023 21:25:10 GMT  
		Size: 2.7 MB (2725026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8ad6c33b9f97d58d2fd510d45a7b5d6cb66ae14565482865f90d9e558a6ec64`  
		Last Modified: Sat, 11 Feb 2023 05:43:06 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82db5de70f22305fe1764a74a4401b63a52b8836764e02b5267428d091b00a13`  
		Last Modified: Sat, 11 Feb 2023 05:43:13 GMT  
		Size: 77.7 MB (77693873 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ec56a511db238cb6741bc812975d9df350607ec2719bb6e6a70832e2c2b6ba1`  
		Last Modified: Sat, 11 Feb 2023 05:43:06 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c38f584463acea946b979e78cc1647a2243f02c44e51bba0bb3f2922aebe1ad2`  
		Last Modified: Sat, 11 Feb 2023 05:43:06 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.10.10` - linux; 386

```console
$ docker pull vault@sha256:1a28c8bf8cf4b0dd75415491e56b29fdc23630db42af13cb524fb3f0b7b32409
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.1 MB (82067642 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fa167f8e4a8c7e509eca8051e623c19ee0d5bf0d932b1c64c16442eb0561fa20`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:39 GMT
ADD file:d88c188553d983f16407f891790a4e553fda681fa265d89ec12a70ba2f41b0da in / 
# Fri, 10 Feb 2023 21:24:39 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:20:49 GMT
ARG VAULT_VERSION=1.10.10
# Sat, 11 Feb 2023 03:20:50 GMT
# ARGS: VAULT_VERSION=1.10.10
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 03:20:59 GMT
# ARGS: VAULT_VERSION=1.10.10
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 03:20:59 GMT
# ARGS: VAULT_VERSION=1.10.10
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 03:21:00 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 03:21:01 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 03:21:02 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 03:21:04 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 03:21:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 03:21:05 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:84644bcd984e34c8b3bc44d8040b7017495e31100c1f4d726c92b40cf6cf7351`  
		Last Modified: Fri, 10 Feb 2023 21:25:51 GMT  
		Size: 2.8 MB (2835110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd2d4c77feb5d41d44453c0ce86ded00c27e16d6297fbd1f415ac8db5bf37703`  
		Last Modified: Sat, 11 Feb 2023 03:22:20 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:feaadfb33a0f159084848b9f5584d22afecf340140e24f8fbe30f6f899854a9e`  
		Last Modified: Sat, 11 Feb 2023 03:22:29 GMT  
		Size: 79.2 MB (79229327 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ff4da8144435ae43ce4564cf04a1673001be369ba838e3de322645cf03dafc2a`  
		Last Modified: Sat, 11 Feb 2023 03:22:20 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:762d1eeeb1b7e6262e6d01f84a93b7f3ae0923ba643bf0b3ddb6b3f0a746dc44`  
		Last Modified: Sat, 11 Feb 2023 03:22:20 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.11.7`

```console
$ docker pull vault@sha256:d2e4a959ac6269f859a17eca7b31119fa7bff78edc349eace3e1c2eb93a7bd84
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.11.7` - linux; amd64

```console
$ docker pull vault@sha256:3a8c08b80dd33f06e39a1ca6053d596b973b9bdb0783a2ee53618b3055d6a94d
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.3 MB (81252188 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e2fa1795afe1db246d434cf8457b34308fdcfdbef8d1a034527ef0b35e72c0af`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:13:59 GMT
ARG VAULT_VERSION=1.11.7
# Sat, 11 Feb 2023 14:13:59 GMT
# ARGS: VAULT_VERSION=1.11.7
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 14:14:07 GMT
# ARGS: VAULT_VERSION=1.11.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 14:14:08 GMT
# ARGS: VAULT_VERSION=1.11.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 14:14:09 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 14:14:09 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 14:14:09 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 14:14:09 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 14:14:09 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:14:09 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7c9f9fe937139e7106e6cb7fc1dce72c9102dda7c0b1e0ae36694ae29d22eb6a`  
		Last Modified: Sat, 11 Feb 2023 14:15:06 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:18e8eec3dd00eae72a9fef0aea8a1a13de16d60ae3fb38b664ebb92c5145b906`  
		Last Modified: Sat, 11 Feb 2023 14:15:15 GMT  
		Size: 78.4 MB (78419287 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5c7fa8c6c1dfa7b22be8bfbaa16d0eadca24f499f7d4237115e7262b346c66c8`  
		Last Modified: Sat, 11 Feb 2023 14:15:06 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:64217e0a1aa392dda3fe01b826f725f325c2abb32634dcd37183a9e75055b1b1`  
		Last Modified: Sat, 11 Feb 2023 14:15:06 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.11.7` - linux; arm variant v6

```console
$ docker pull vault@sha256:9a3b0f1e33cbae19128ab9361d5e9c21c3e735296f351d5338a9d88a3419d07f
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.3 MB (76337080 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b2f41adbae28f85e9508b941555531513dcfee6046abb5119ce0b449e6ac6632`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:41 GMT
ADD file:767f6566ea2c075838c0a86ca644a37e446f309f68952f5f921970f046abd252 in / 
# Fri, 10 Feb 2023 20:49:41 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:35:34 GMT
ARG VAULT_VERSION=1.11.7
# Sat, 11 Feb 2023 03:35:35 GMT
# ARGS: VAULT_VERSION=1.11.7
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 03:35:43 GMT
# ARGS: VAULT_VERSION=1.11.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 03:35:44 GMT
# ARGS: VAULT_VERSION=1.11.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 03:35:44 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 03:35:44 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 03:35:44 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 03:35:44 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 03:35:44 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 03:35:45 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7616dd32f4bf5fddffb2543afaac2355a5fc495348c01060cd67181e36343e96`  
		Last Modified: Fri, 10 Feb 2023 20:51:02 GMT  
		Size: 2.6 MB (2638152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e13db9cf6402614e4fa07861269aa23e0581bfd875f3346eb2b696d5be8e0ff`  
		Last Modified: Sat, 11 Feb 2023 03:37:03 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:370a13af74b8980409b5d524d20c729af901e1100b3c7b71d37cc4adbdf5d31e`  
		Last Modified: Sat, 11 Feb 2023 03:37:14 GMT  
		Size: 73.7 MB (73695721 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdac7772d2dcd4b577b962e135047d6e9f92a17e7b9934bd524d13a6cc6655e1`  
		Last Modified: Sat, 11 Feb 2023 03:37:03 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea9d9eb13cbdfe9b10d4f5f682473619bbf9b4abe67eddb4e26cdd39a8d8e298`  
		Last Modified: Sat, 11 Feb 2023 03:37:03 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.11.7` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:2f30512a958296b617d73efd1dfec0e7287c0478ab7882d486b9ee7d38376d13
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.5 MB (76536770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bb684f5e2ff8b198ae21529b959bb2ead2a12231a306eaec304aa2dea832f502`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:19 GMT
ADD file:50a841463966858f1c3ca87143cf96145d1d52f7349ef516adfbf21cdd5684fe in / 
# Fri, 10 Feb 2023 21:24:19 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:41:49 GMT
ARG VAULT_VERSION=1.11.7
# Sat, 11 Feb 2023 05:41:50 GMT
# ARGS: VAULT_VERSION=1.11.7
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 05:41:56 GMT
# ARGS: VAULT_VERSION=1.11.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 05:41:58 GMT
# ARGS: VAULT_VERSION=1.11.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 05:41:58 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 05:41:58 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 05:41:58 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 05:41:58 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 05:41:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:41:58 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:6f0e733d82e26042c603e231c39b56abbabdad66673a736ec71c69c65be95f41`  
		Last Modified: Fri, 10 Feb 2023 21:25:10 GMT  
		Size: 2.7 MB (2725026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb51d7030abd44604873502bc49bed67747b21a34f7814d85deb840d9b541831`  
		Last Modified: Sat, 11 Feb 2023 05:42:54 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b40a50ac2bfe74426b71d29289e22f29039eb853fa940bc2dd4395325522056f`  
		Last Modified: Sat, 11 Feb 2023 05:43:00 GMT  
		Size: 73.8 MB (73808472 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b268f097dfc39d9cca767b2779a07545a01c028a8964f61f2b4029a2104b5513`  
		Last Modified: Sat, 11 Feb 2023 05:42:54 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:55d0bc175730f16ae74916c023ead51c411804c3114ac72508608d8aae3b89ae`  
		Last Modified: Sat, 11 Feb 2023 05:42:54 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.11.7` - linux; 386

```console
$ docker pull vault@sha256:5631136b4260a5d30940d18b21f8af3f72e2773b6fcef0a65ad87bf8754be313
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.0 MB (78042931 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:49d523c764deb44599825acebfeb52fe2ee8da849af124841bd7b4b8bba43291`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:39 GMT
ADD file:d88c188553d983f16407f891790a4e553fda681fa265d89ec12a70ba2f41b0da in / 
# Fri, 10 Feb 2023 21:24:39 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:20:26 GMT
ARG VAULT_VERSION=1.11.7
# Sat, 11 Feb 2023 03:20:27 GMT
# ARGS: VAULT_VERSION=1.11.7
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 03:20:36 GMT
# ARGS: VAULT_VERSION=1.11.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 03:20:36 GMT
# ARGS: VAULT_VERSION=1.11.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 03:20:37 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 03:20:38 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 03:20:39 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 03:20:41 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 03:20:41 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 03:20:42 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:84644bcd984e34c8b3bc44d8040b7017495e31100c1f4d726c92b40cf6cf7351`  
		Last Modified: Fri, 10 Feb 2023 21:25:51 GMT  
		Size: 2.8 MB (2835110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1816e10dd810d644a0fb367487b5524c6699f1327299a1a0ffac7eb9278884c`  
		Last Modified: Sat, 11 Feb 2023 03:22:05 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f5cd78e3476bbfd919c13e7706b18ca8d7808ac80169d3a99d40153618d98c3`  
		Last Modified: Sat, 11 Feb 2023 03:22:13 GMT  
		Size: 75.2 MB (75204613 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e4df94298c412c42110ee4156d9076bdc12fc838a6461e38fffd102250b409e`  
		Last Modified: Sat, 11 Feb 2023 03:22:05 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3343fa4b2c4e1043c9a2fd76effe2bdd147bd7da89c37f68140c010ceeb87b9`  
		Last Modified: Sat, 11 Feb 2023 03:22:05 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.12.3`

```console
$ docker pull vault@sha256:41467bd2a3bf4a2b619e286be2fa7906e8e0db234e6cb3d602bbb8f40308da49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.12.3` - linux; amd64

```console
$ docker pull vault@sha256:948f477f6b527845ccfe037df99aaf4f2c7188044aa161009fadc5caadb938c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.0 MB (85985608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4ff36f465aef5d588443f04c07ad56dd543948bb99836d165dc826f9e0dccee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:13:45 GMT
ARG VAULT_VERSION=1.12.3
# Sat, 11 Feb 2023 14:13:45 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 14:13:54 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 14:13:55 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 14:13:55 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 14:13:55 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 14:13:55 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 14:13:55 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 14:13:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:13:55 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9cc71da9cbb3ba5068f26fb4128aa5106962388acb933b26ff2a0ebf33312a`  
		Last Modified: Sat, 11 Feb 2023 14:14:47 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b356f0a9251efd9340ab50a4b5a506603ad35b7c2613831b7d8dd050514dda`  
		Last Modified: Sat, 11 Feb 2023 14:14:57 GMT  
		Size: 83.2 MB (83152706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6055efb8ab6fdbc45aa89f7036bd4de80d2d0327c50ed119e3c381caaf0eeb`  
		Last Modified: Sat, 11 Feb 2023 14:14:47 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b84c2c36b75e34b959cf5db2f90767bcc2e40787b3c8999be16fdb6e5a5988`  
		Last Modified: Sat, 11 Feb 2023 14:14:47 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.12.3` - linux; arm variant v6

```console
$ docker pull vault@sha256:1e94f96b0f75676aefb39c2007c9186d58ed6a8dcc9bca58853adc2d110d09ec
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.7 MB (80690756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38370d9dc64624127cab2f31df8f8dd8f03f6f0618b570bac89988a460f23231`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:41 GMT
ADD file:767f6566ea2c075838c0a86ca644a37e446f309f68952f5f921970f046abd252 in / 
# Fri, 10 Feb 2023 20:49:41 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:35:14 GMT
ARG VAULT_VERSION=1.12.3
# Sat, 11 Feb 2023 03:35:15 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 03:35:27 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 03:35:28 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 03:35:28 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 03:35:28 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 03:35:28 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 03:35:28 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 03:35:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 03:35:28 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7616dd32f4bf5fddffb2543afaac2355a5fc495348c01060cd67181e36343e96`  
		Last Modified: Fri, 10 Feb 2023 20:51:02 GMT  
		Size: 2.6 MB (2638152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a248407323953611931dabb84c2a90b0802a92f52f7631be273a66a0115c7f`  
		Last Modified: Sat, 11 Feb 2023 03:36:41 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5ecfb0e18a0a56ae61ec5314a08ea2d6519176c62382c7eb59d0611ecfbd33`  
		Last Modified: Sat, 11 Feb 2023 03:36:52 GMT  
		Size: 78.0 MB (78049395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3b0f87410a36d660fe2e5788634a86f1cf02fff3131856a278b08b2e2e4b91`  
		Last Modified: Sat, 11 Feb 2023 03:36:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1508cd5e112dd20424639b3373266d8abf7e3d5acbd6bdcf880f214eb57c0b5e`  
		Last Modified: Sat, 11 Feb 2023 03:36:41 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.12.3` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:792fe16e9303fd48382de3c0b537c317140f1fe652c7c4f5072dbbd9d8c2ce5a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (81032801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a053d50c41ec09d93790c8b3e70965bb3921f1c3e040976b7c349dbd757d356e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:19 GMT
ADD file:50a841463966858f1c3ca87143cf96145d1d52f7349ef516adfbf21cdd5684fe in / 
# Fri, 10 Feb 2023 21:24:19 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:41:36 GMT
ARG VAULT_VERSION=1.12.3
# Sat, 11 Feb 2023 05:41:36 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 05:41:44 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 05:41:46 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 05:41:46 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 05:41:46 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 05:41:46 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 05:41:46 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 05:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:41:46 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:6f0e733d82e26042c603e231c39b56abbabdad66673a736ec71c69c65be95f41`  
		Last Modified: Fri, 10 Feb 2023 21:25:10 GMT  
		Size: 2.7 MB (2725026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55a63a3942e9a89216e8c5b6b929390e729f15d178980dd6ffcec3857c27f38`  
		Last Modified: Sat, 11 Feb 2023 05:42:38 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88570abe2214b26aaacfed509cb161606d15bc69ff0eb471181e29b8a9207e95`  
		Last Modified: Sat, 11 Feb 2023 05:42:46 GMT  
		Size: 78.3 MB (78304503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5dd61ea579410543ec13ecf60853a5de6d1671145aa5f2803b643946877927`  
		Last Modified: Sat, 11 Feb 2023 05:42:38 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77575e24089e446aac7dc19348333fb6229c46899d78ab611d3695163d93529`  
		Last Modified: Sat, 11 Feb 2023 05:42:38 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.12.3` - linux; 386

```console
$ docker pull vault@sha256:e455ff516a8e67750f6f43c52118b8fbc7370c4e2c4485943ac28d7a1af1cd2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.4 MB (82438567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:568ac2a776af5fdc263849f1462a14095ddfdae3e0d617c925043dc5ac004ca4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:39 GMT
ADD file:d88c188553d983f16407f891790a4e553fda681fa265d89ec12a70ba2f41b0da in / 
# Fri, 10 Feb 2023 21:24:39 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:20:03 GMT
ARG VAULT_VERSION=1.12.3
# Sat, 11 Feb 2023 03:20:04 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 03:20:14 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 03:20:14 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 03:20:15 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 03:20:16 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 03:20:17 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 03:20:19 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 03:20:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 03:20:20 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:84644bcd984e34c8b3bc44d8040b7017495e31100c1f4d726c92b40cf6cf7351`  
		Last Modified: Fri, 10 Feb 2023 21:25:51 GMT  
		Size: 2.8 MB (2835110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8d2bb6e4c083ab6b5cf6f5f088214983e1b4770736e1e1e11471adb5abfa21`  
		Last Modified: Sat, 11 Feb 2023 03:21:47 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd9d406cdb741f3514a9619da54bbfbe7e70cc88b3d62adf4d52c1157ffb04d`  
		Last Modified: Sat, 11 Feb 2023 03:21:55 GMT  
		Size: 79.6 MB (79600251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63462961af4d9764794a5b43c2436f43d81626e0943972a9b3f1880eccd86e61`  
		Last Modified: Sat, 11 Feb 2023 03:21:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5b862971ae4e8956b1790208ebb629a1af5662104873b36edb362be50fcd4d`  
		Last Modified: Sat, 11 Feb 2023 03:21:47 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.9.10`

```console
$ docker pull vault@sha256:0d9934eab2c599bfa7a51417e7ea80c7daea2a445825a5b286c1693b5c9b512c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.9.10` - linux; amd64

```console
$ docker pull vault@sha256:55b29d23a3a2dcf26ff4939c73f01b461703cc16d4c3ac67ef2cdbad32daf0c0
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.2 MB (73195437 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2316398b0e242e494f42f954a5860c4015d5cced51ef3abf33eb431f36b94869`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:14:27 GMT
ARG VAULT_VERSION=1.9.10
# Sat, 11 Feb 2023 14:14:28 GMT
# ARGS: VAULT_VERSION=1.9.10
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 14:14:35 GMT
# ARGS: VAULT_VERSION=1.9.10
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 14:14:36 GMT
# ARGS: VAULT_VERSION=1.9.10
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 14:14:36 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 14:14:36 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 14:14:36 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 14:14:36 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 14:14:36 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:14:36 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:42adfe0583a95bae77c56c2bf15371b74f461cda1fb3fa07f077a9baabb465f0`  
		Last Modified: Sat, 11 Feb 2023 14:15:36 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5c0a932a3faba08bd05d19a3e2d0be31731b6aab4e29e8323b991dd76d398f7`  
		Last Modified: Sat, 11 Feb 2023 14:15:45 GMT  
		Size: 70.4 MB (70362536 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8756bf5050be6dc280a2fb5757039c287d0d3f3d88d20ce4483078da6958632`  
		Last Modified: Sat, 11 Feb 2023 14:15:36 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a01e50c79370eaf698645b343ad636f6afd24e032e65a722d620bb99f8ebc68`  
		Last Modified: Sat, 11 Feb 2023 14:15:36 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.10` - linux; arm variant v6

```console
$ docker pull vault@sha256:0b55b3a6d51ff3bcaeada0f5ee7764bf2a86202c8c0a42981037905fb26c68bf
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.5 MB (66517431 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a414752273a01ec4f29a97b4e0ba9ae917286e492eec80b2828fbbf975208181`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:41 GMT
ADD file:767f6566ea2c075838c0a86ca644a37e446f309f68952f5f921970f046abd252 in / 
# Fri, 10 Feb 2023 20:49:41 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:36:08 GMT
ARG VAULT_VERSION=1.9.10
# Sat, 11 Feb 2023 03:36:09 GMT
# ARGS: VAULT_VERSION=1.9.10
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 03:36:18 GMT
# ARGS: VAULT_VERSION=1.9.10
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 03:36:20 GMT
# ARGS: VAULT_VERSION=1.9.10
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 03:36:20 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 03:36:20 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 03:36:20 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 03:36:20 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 03:36:20 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 03:36:20 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7616dd32f4bf5fddffb2543afaac2355a5fc495348c01060cd67181e36343e96`  
		Last Modified: Fri, 10 Feb 2023 20:51:02 GMT  
		Size: 2.6 MB (2638152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d626305bcd21d9a363de822c34d2ab96d7e748bde96536d0ae5a942f08ec9b7`  
		Last Modified: Sat, 11 Feb 2023 03:37:42 GMT  
		Size: 1.2 KB (1239 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6fd65c8eb8708997f208abfea2fcf2df338c2a1e6ce2591ba5b8efa3e74997e`  
		Last Modified: Sat, 11 Feb 2023 03:37:52 GMT  
		Size: 63.9 MB (63876072 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:06a192e6a19ca1ce2c0bbf0e38cf88c2a968abc17b7e2b738b3d3ef1a64f4c25`  
		Last Modified: Sat, 11 Feb 2023 03:37:42 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:201d361e85fa7b10cd51a83ce405a13873c2d15bb0cc6f2c4819a7185814d829`  
		Last Modified: Sat, 11 Feb 2023 03:37:42 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.10` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:0a7e3d0e9756a48fb2dffa366dfbed5f991955bdd9e9550667a0f45465e41e19
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.3 MB (68308676 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5e5478979ab741d2344f01aea97d43cfc8b0c99c731f92055cec53ab23f0f6ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:19 GMT
ADD file:50a841463966858f1c3ca87143cf96145d1d52f7349ef516adfbf21cdd5684fe in / 
# Fri, 10 Feb 2023 21:24:19 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:42:15 GMT
ARG VAULT_VERSION=1.9.10
# Sat, 11 Feb 2023 05:42:15 GMT
# ARGS: VAULT_VERSION=1.9.10
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 05:42:23 GMT
# ARGS: VAULT_VERSION=1.9.10
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 05:42:24 GMT
# ARGS: VAULT_VERSION=1.9.10
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 05:42:24 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 05:42:24 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 05:42:24 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 05:42:25 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 05:42:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:42:25 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:6f0e733d82e26042c603e231c39b56abbabdad66673a736ec71c69c65be95f41`  
		Last Modified: Fri, 10 Feb 2023 21:25:10 GMT  
		Size: 2.7 MB (2725026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5da1299c7c17200806384c64889d9f02e4de344fe7c94d728a39abad833d15a9`  
		Last Modified: Sat, 11 Feb 2023 05:43:19 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e104ca9fdae73837d6425e652269ebb5bfe63d4eb940004dd7e4b658273425d`  
		Last Modified: Sat, 11 Feb 2023 05:43:26 GMT  
		Size: 65.6 MB (65580379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e903f1611ec541ff9c37019fe9384ad7d34216d2422e68211ae673048f764851`  
		Last Modified: Sat, 11 Feb 2023 05:43:19 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:766f7b44db45cd117107a8d2ba5c6f8323cc808d2a432df8292a4d960929cbed`  
		Last Modified: Sat, 11 Feb 2023 05:43:19 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.9.10` - linux; 386

```console
$ docker pull vault@sha256:0796e2d2be6a6d401d66020b71832cc08b95079e8b182a6f6dc5fe95eb0c9a67
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.6 MB (69567212 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0380bd81ebdb87cec0c79d219fd4eb3b7587fc9831db30f70c702346aefdf66d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:39 GMT
ADD file:d88c188553d983f16407f891790a4e553fda681fa265d89ec12a70ba2f41b0da in / 
# Fri, 10 Feb 2023 21:24:39 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:21:11 GMT
ARG VAULT_VERSION=1.9.10
# Sat, 11 Feb 2023 03:21:12 GMT
# ARGS: VAULT_VERSION=1.9.10
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 03:21:21 GMT
# ARGS: VAULT_VERSION=1.9.10
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 03:21:21 GMT
# ARGS: VAULT_VERSION=1.9.10
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 03:21:22 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 03:21:23 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 03:21:24 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 03:21:26 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 03:21:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 03:21:27 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:84644bcd984e34c8b3bc44d8040b7017495e31100c1f4d726c92b40cf6cf7351`  
		Last Modified: Fri, 10 Feb 2023 21:25:51 GMT  
		Size: 2.8 MB (2835110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:293ece0120874ec766df296e65d51a7d8cc13921da7c4b6f45b610908238f035`  
		Last Modified: Sat, 11 Feb 2023 03:22:36 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2aa4386856290235a6cf8b50a6b8e22e9ca26d8a15fb136ae3ec0a98bb32d2fe`  
		Last Modified: Sat, 11 Feb 2023 03:22:44 GMT  
		Size: 66.7 MB (66728896 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23034eac9ead4e14ad22eeaf3d94ae8e2ea01a7f993cf439445a1701295149f`  
		Last Modified: Sat, 11 Feb 2023 03:22:36 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:715f9b0bccea6507fda7c7103c9b03b83a5489161d9c9e8c5c032dab444d1527`  
		Last Modified: Sat, 11 Feb 2023 03:22:36 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:41467bd2a3bf4a2b619e286be2fa7906e8e0db234e6cb3d602bbb8f40308da49
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:948f477f6b527845ccfe037df99aaf4f2c7188044aa161009fadc5caadb938c1
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.0 MB (85985608 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d4ff36f465aef5d588443f04c07ad56dd543948bb99836d165dc826f9e0dccee`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:59 GMT
ADD file:a41bb436701fd0adf99a3157d19f172b3e54ea033f5c617009e2d1bdeac206d7 in / 
# Sat, 11 Feb 2023 04:46:59 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 14:13:45 GMT
ARG VAULT_VERSION=1.12.3
# Sat, 11 Feb 2023 14:13:45 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 14:13:54 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 14:13:55 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 14:13:55 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 14:13:55 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 14:13:55 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 14:13:55 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 14:13:55 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 14:13:55 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:d261077062b2aebb9ca8dc61f2b00e7e2b4e44179d3cfbe526c4ee0c5e41b26f`  
		Last Modified: Sat, 11 Feb 2023 04:47:49 GMT  
		Size: 2.8 MB (2829633 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aa9cc71da9cbb3ba5068f26fb4128aa5106962388acb933b26ff2a0ebf33312a`  
		Last Modified: Sat, 11 Feb 2023 14:14:47 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:36b356f0a9251efd9340ab50a4b5a506603ad35b7c2613831b7d8dd050514dda`  
		Last Modified: Sat, 11 Feb 2023 14:14:57 GMT  
		Size: 83.2 MB (83152706 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6e6055efb8ab6fdbc45aa89f7036bd4de80d2d0327c50ed119e3c381caaf0eeb`  
		Last Modified: Sat, 11 Feb 2023 14:14:47 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3b84c2c36b75e34b959cf5db2f90767bcc2e40787b3c8999be16fdb6e5a5988`  
		Last Modified: Sat, 11 Feb 2023 14:14:47 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:1e94f96b0f75676aefb39c2007c9186d58ed6a8dcc9bca58853adc2d110d09ec
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **80.7 MB (80690756 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38370d9dc64624127cab2f31df8f8dd8f03f6f0618b570bac89988a460f23231`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 10 Feb 2023 20:49:41 GMT
ADD file:767f6566ea2c075838c0a86ca644a37e446f309f68952f5f921970f046abd252 in / 
# Fri, 10 Feb 2023 20:49:41 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:35:14 GMT
ARG VAULT_VERSION=1.12.3
# Sat, 11 Feb 2023 03:35:15 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 03:35:27 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 03:35:28 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 03:35:28 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 03:35:28 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 03:35:28 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 03:35:28 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 03:35:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 03:35:28 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:7616dd32f4bf5fddffb2543afaac2355a5fc495348c01060cd67181e36343e96`  
		Last Modified: Fri, 10 Feb 2023 20:51:02 GMT  
		Size: 2.6 MB (2638152 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3a248407323953611931dabb84c2a90b0802a92f52f7631be273a66a0115c7f`  
		Last Modified: Sat, 11 Feb 2023 03:36:41 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7e5ecfb0e18a0a56ae61ec5314a08ea2d6519176c62382c7eb59d0611ecfbd33`  
		Last Modified: Sat, 11 Feb 2023 03:36:52 GMT  
		Size: 78.0 MB (78049395 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb3b0f87410a36d660fe2e5788634a86f1cf02fff3131856a278b08b2e2e4b91`  
		Last Modified: Sat, 11 Feb 2023 03:36:41 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1508cd5e112dd20424639b3373266d8abf7e3d5acbd6bdcf880f214eb57c0b5e`  
		Last Modified: Sat, 11 Feb 2023 03:36:41 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:792fe16e9303fd48382de3c0b537c317140f1fe652c7c4f5072dbbd9d8c2ce5a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.0 MB (81032801 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a053d50c41ec09d93790c8b3e70965bb3921f1c3e040976b7c349dbd757d356e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:19 GMT
ADD file:50a841463966858f1c3ca87143cf96145d1d52f7349ef516adfbf21cdd5684fe in / 
# Fri, 10 Feb 2023 21:24:19 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 05:41:36 GMT
ARG VAULT_VERSION=1.12.3
# Sat, 11 Feb 2023 05:41:36 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 05:41:44 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 05:41:46 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 05:41:46 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 05:41:46 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 05:41:46 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 05:41:46 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 05:41:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 05:41:46 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:6f0e733d82e26042c603e231c39b56abbabdad66673a736ec71c69c65be95f41`  
		Last Modified: Fri, 10 Feb 2023 21:25:10 GMT  
		Size: 2.7 MB (2725026 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b55a63a3942e9a89216e8c5b6b929390e729f15d178980dd6ffcec3857c27f38`  
		Last Modified: Sat, 11 Feb 2023 05:42:38 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:88570abe2214b26aaacfed509cb161606d15bc69ff0eb471181e29b8a9207e95`  
		Last Modified: Sat, 11 Feb 2023 05:42:46 GMT  
		Size: 78.3 MB (78304503 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7a5dd61ea579410543ec13ecf60853a5de6d1671145aa5f2803b643946877927`  
		Last Modified: Sat, 11 Feb 2023 05:42:38 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a77575e24089e446aac7dc19348333fb6229c46899d78ab611d3695163d93529`  
		Last Modified: Sat, 11 Feb 2023 05:42:38 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:e455ff516a8e67750f6f43c52118b8fbc7370c4e2c4485943ac28d7a1af1cd2c
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.4 MB (82438567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:568ac2a776af5fdc263849f1462a14095ddfdae3e0d617c925043dc5ac004ca4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 10 Feb 2023 21:24:39 GMT
ADD file:d88c188553d983f16407f891790a4e553fda681fa265d89ec12a70ba2f41b0da in / 
# Fri, 10 Feb 2023 21:24:39 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 03:20:03 GMT
ARG VAULT_VERSION=1.12.3
# Sat, 11 Feb 2023 03:20:04 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN addgroup vault &&     adduser -S -G vault vault
# Sat, 11 Feb 2023 03:20:14 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Sat, 11 Feb 2023 03:20:14 GMT
# ARGS: VAULT_VERSION=1.12.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Sat, 11 Feb 2023 03:20:15 GMT
VOLUME [/vault/logs]
# Sat, 11 Feb 2023 03:20:16 GMT
VOLUME [/vault/file]
# Sat, 11 Feb 2023 03:20:17 GMT
EXPOSE 8200
# Sat, 11 Feb 2023 03:20:19 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Sat, 11 Feb 2023 03:20:19 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Sat, 11 Feb 2023 03:20:20 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:84644bcd984e34c8b3bc44d8040b7017495e31100c1f4d726c92b40cf6cf7351`  
		Last Modified: Fri, 10 Feb 2023 21:25:51 GMT  
		Size: 2.8 MB (2835110 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6d8d2bb6e4c083ab6b5cf6f5f088214983e1b4770736e1e1e11471adb5abfa21`  
		Last Modified: Sat, 11 Feb 2023 03:21:47 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5dd9d406cdb741f3514a9619da54bbfbe7e70cc88b3d62adf4d52c1157ffb04d`  
		Last Modified: Sat, 11 Feb 2023 03:21:55 GMT  
		Size: 79.6 MB (79600251 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:63462961af4d9764794a5b43c2436f43d81626e0943972a9b3f1880eccd86e61`  
		Last Modified: Sat, 11 Feb 2023 03:21:47 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fa5b862971ae4e8956b1790208ebb629a1af5662104873b36edb362be50fcd4d`  
		Last Modified: Sat, 11 Feb 2023 03:21:47 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
