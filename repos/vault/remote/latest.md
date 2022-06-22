## `vault:latest`

```console
$ docker pull vault@sha256:d45ffca3b9bc5f15f665c0afb581de668bca935ff1fffa10049648183c80ef6f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:28c17b49e4abe0a02337a14cfe2b38c39ff7f72f173245734e77f5d606a438ce
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.4 MB (77436251 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3bdb60d335ce6c24477dfc464ab96b7b714efc0a3a73c91c84e0f1d92b3dbc2f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Tue, 05 Apr 2022 00:20:08 GMT
ADD file:b9eae64dc6ab27fdaa048b7cda06fcb5c7655e1b327e098e2775d095cb657b01 in / 
# Tue, 05 Apr 2022 00:20:08 GMT
CMD ["/bin/sh"]
# Wed, 22 Jun 2022 02:37:09 GMT
ARG VAULT_VERSION=1.11.0
# Wed, 22 Jun 2022 02:37:09 GMT
# ARGS: VAULT_VERSION=1.11.0
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Jun 2022 02:37:17 GMT
# ARGS: VAULT_VERSION=1.11.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Jun 2022 02:37:18 GMT
# ARGS: VAULT_VERSION=1.11.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Jun 2022 02:37:18 GMT
VOLUME [/vault/logs]
# Wed, 22 Jun 2022 02:37:18 GMT
VOLUME [/vault/file]
# Wed, 22 Jun 2022 02:37:18 GMT
EXPOSE 8200
# Wed, 22 Jun 2022 02:37:18 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Jun 2022 02:37:18 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jun 2022 02:37:19 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8663204ce13b2961da55026a2034abb9e5afaaccf6a9cfb44ad71406dcd07c7b`  
		Last Modified: Tue, 05 Apr 2022 00:20:51 GMT  
		Size: 2.8 MB (2818370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1f4d45ca1b2ac54593aeb87408785af026f4f1ce21b567c008c1effaf359e5b4`  
		Last Modified: Wed, 22 Jun 2022 02:37:35 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7459aeb2a3199abbd8d479cd2c0122e91e193f8af34e5b46a1aa8908a42b80f1`  
		Last Modified: Wed, 22 Jun 2022 02:37:44 GMT  
		Size: 74.6 MB (74614607 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f019a19c088e4a6bf942b34673aac2a116a9ad8ef222ad2396307817d9b03fb`  
		Last Modified: Wed, 22 Jun 2022 02:37:35 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22616ff81410691d7e521e21bd1ef72f70ad1e49e424d0b5be71d1e267a9f7fe`  
		Last Modified: Wed, 22 Jun 2022 02:37:35 GMT  
		Size: 1.8 KB (1816 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:ae7d7b19458c2e2566623e6a32d2ac39e68ca72af02c596fa875c364f3d52184
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.2 MB (70208271 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:745c6f428116885bb53b0e56bf6895d53b8c181f02c3511f4480034a337fbaeb`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Mon, 04 Apr 2022 23:49:55 GMT
ADD file:2e4db0cea3f5eecfbb82c5abd09eb100749fed0189fc30d2c51980d2560e3ccb in / 
# Mon, 04 Apr 2022 23:49:56 GMT
CMD ["/bin/sh"]
# Tue, 21 Jun 2022 23:51:06 GMT
ARG VAULT_VERSION=1.11.0
# Tue, 21 Jun 2022 23:51:08 GMT
# ARGS: VAULT_VERSION=1.11.0
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 21 Jun 2022 23:51:27 GMT
# ARGS: VAULT_VERSION=1.11.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 21 Jun 2022 23:51:30 GMT
# ARGS: VAULT_VERSION=1.11.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 21 Jun 2022 23:51:30 GMT
VOLUME [/vault/logs]
# Tue, 21 Jun 2022 23:51:30 GMT
VOLUME [/vault/file]
# Tue, 21 Jun 2022 23:51:31 GMT
EXPOSE 8200
# Tue, 21 Jun 2022 23:51:31 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 21 Jun 2022 23:51:32 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 21 Jun 2022 23:51:32 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f9f2e4e531ad51ee917e8311e91a223a4893c1d754acb8246af87375ea60c6aa`  
		Last Modified: Mon, 04 Apr 2022 23:51:47 GMT  
		Size: 2.6 MB (2626056 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61510bfcfaebed522571694f06bc8e6f60afdbfe5928246f5007c7e8e03bd500`  
		Last Modified: Tue, 21 Jun 2022 23:52:29 GMT  
		Size: 1.3 KB (1268 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b2d1e980fe553c83740bb98b55b61f089aa8fdb053622f7021e042ec9bccdf4`  
		Last Modified: Tue, 21 Jun 2022 23:53:06 GMT  
		Size: 67.6 MB (67578948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:938218f9a2801982962aa75e217eb4d0e5f5e968f6e1342200647380d6db7b12`  
		Last Modified: Tue, 21 Jun 2022 23:52:29 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:289b1df03577decc3cb73f38551da8e247922f1ffe3a66bc7c7e05ace23a9cc4`  
		Last Modified: Tue, 21 Jun 2022 23:52:29 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:810ded0e55ab1d0b8fa57bc7060c071945c79f086bbd413101ba446f03bd3aa6
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.3 MB (72252336 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:fc1951f8812bf1c51db0a42edf1bbed44a263d3bea537d025fc368e2aa29e49a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Mon, 04 Apr 2022 23:39:39 GMT
ADD file:66f473ec586f45376eb1941936c7829f636b90cad2022233cacf3186ac747ef9 in / 
# Mon, 04 Apr 2022 23:39:39 GMT
CMD ["/bin/sh"]
# Wed, 22 Jun 2022 03:17:09 GMT
ARG VAULT_VERSION=1.11.0
# Wed, 22 Jun 2022 03:17:10 GMT
# ARGS: VAULT_VERSION=1.11.0
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Jun 2022 03:17:19 GMT
# ARGS: VAULT_VERSION=1.11.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Jun 2022 03:17:20 GMT
# ARGS: VAULT_VERSION=1.11.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Jun 2022 03:17:21 GMT
VOLUME [/vault/logs]
# Wed, 22 Jun 2022 03:17:22 GMT
VOLUME [/vault/file]
# Wed, 22 Jun 2022 03:17:23 GMT
EXPOSE 8200
# Wed, 22 Jun 2022 03:17:25 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Jun 2022 03:17:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jun 2022 03:17:26 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:455c02918c4592a9beeeae47df541266f3ea53ed573feb767e5e8ab8dcee146e`  
		Last Modified: Mon, 04 Apr 2022 23:40:41 GMT  
		Size: 2.7 MB (2717389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:10ec8b7e7fc35cf2f287ea02c195d99090ae431c4aa4e66c31a2f8e58ef66fec`  
		Last Modified: Wed, 22 Jun 2022 03:17:56 GMT  
		Size: 1.2 KB (1237 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f25bda75901f25501bca193e34ef0bfba67636bf2edd90f687dba610a6a48087`  
		Last Modified: Wed, 22 Jun 2022 03:18:07 GMT  
		Size: 69.5 MB (69531741 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0b092a015fb79c9f94c5d3e8b1d5714ca072d6d2e22fc5557bfe60ac359c67`  
		Last Modified: Wed, 22 Jun 2022 03:17:56 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc4a35fc984c96a1d024f43ee8eb6b8e020d104d092d954b29b65d96fd633674`  
		Last Modified: Wed, 22 Jun 2022 03:17:56 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:255c5437a7b1d8a3aea09a9613ef4452a4be17b243e2feb586a89f001262789a
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **73.5 MB (73513567 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0a4eb42320384031bc8fca7e8aac129513ed145980f4339f8d503256b63d393`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Mon, 04 Apr 2022 23:38:32 GMT
ADD file:6508514d43b69774a3307679ef8f6dba0faf707e62ad6c6c1c8cf40d84e12d1d in / 
# Mon, 04 Apr 2022 23:38:32 GMT
CMD ["/bin/sh"]
# Wed, 22 Jun 2022 02:24:26 GMT
ARG VAULT_VERSION=1.11.0
# Wed, 22 Jun 2022 02:24:27 GMT
# ARGS: VAULT_VERSION=1.11.0
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Jun 2022 02:24:37 GMT
# ARGS: VAULT_VERSION=1.11.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Jun 2022 02:24:37 GMT
# ARGS: VAULT_VERSION=1.11.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Jun 2022 02:24:38 GMT
VOLUME [/vault/logs]
# Wed, 22 Jun 2022 02:24:39 GMT
VOLUME [/vault/file]
# Wed, 22 Jun 2022 02:24:40 GMT
EXPOSE 8200
# Wed, 22 Jun 2022 02:24:42 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Jun 2022 02:24:42 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Jun 2022 02:24:43 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:c11e5e1035714514f6e237dffd1836a4d03b48af64e55a8e08f9bd9e998e24a9`  
		Last Modified: Mon, 04 Apr 2022 23:39:35 GMT  
		Size: 2.8 MB (2821213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a389d7c654b0df7ef8cd6eaecbf3f30f9701da671ac012f58704a102f1ab87d`  
		Last Modified: Wed, 22 Jun 2022 02:25:13 GMT  
		Size: 1.2 KB (1240 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f213ed344788709165791b60ca93d45117f799b40a693e6c7851923e8eec5871`  
		Last Modified: Wed, 22 Jun 2022 02:25:27 GMT  
		Size: 70.7 MB (70689145 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b52bacb022869b0c17b8055ba990d56af7ceb626265fe46ff1ec0649b792b2d`  
		Last Modified: Wed, 22 Jun 2022 02:25:13 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:184772aa0c3a8b66ff18ba4c4dd3ee278d771b6fe66c1044fedb1d368138e101`  
		Last Modified: Wed, 22 Jun 2022 02:25:13 GMT  
		Size: 1.8 KB (1815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
