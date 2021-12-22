## `vault:latest`

```console
$ docker pull vault@sha256:cc7bca14ebe2e6f32401bf5e59c1b95081c387b75fb0c06c18c085670338a59b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:120f43bbc0ee041245631b78e6287e93861ae73674c034e4882bdc30290cf638
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.9 MB (72932445 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9bb605f7fffed3a5db4aaa27c80eb0c9b5de898356ebf5e66c7897fce56f29f3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 17:19:44 GMT
ADD file:762c899ec0505d1a32930ee804c5b008825f41611161be104076cba33b7e5b2b in / 
# Fri, 12 Nov 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 22:02:49 GMT
ARG VAULT_VERSION=1.9.2
# Wed, 22 Dec 2021 22:02:50 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 22:02:58 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 22:02:59 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 22:02:59 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 22:02:59 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 22:03:00 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 22:03:00 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 22:03:00 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 22:03:00 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:97518928ae5f3d52d4164b314a7e73654eb686ecd8aafa0b79acd980773a740d`  
		Last Modified: Fri, 12 Nov 2021 17:20:39 GMT  
		Size: 2.8 MB (2822981 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:250eba83471e864023d238d7abbb96696bda8bda36f593f865b2aba942906be5`  
		Last Modified: Wed, 22 Dec 2021 22:03:39 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0778ed8dc3c55ba6c08cdb43c8de991ab5aedaa82eaad0489d1f2df7275223`  
		Last Modified: Wed, 22 Dec 2021 22:03:48 GMT  
		Size: 70.1 MB (70106184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:04235f19b893279594f8e24d437da5a44d33c0631925aabad650223253f7c302`  
		Last Modified: Wed, 22 Dec 2021 22:03:39 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd4279ec1af0bf74afd5930fccefe77382fecb716f683ca466e18184fd8b2971`  
		Last Modified: Wed, 22 Dec 2021 22:03:39 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:76b197761a6bf77dfb6940f47db781306b0e4a99bfe395ca4669ff664bbb5291
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.3 MB (66295841 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f1ba640002891c65168c01e7a6e1b8cec7febed127e265b4379ef85cbc7c9916`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:49:42 GMT
ADD file:6daf1fe862c00673bf9cf4d7e20b0bf253a56e7fb8ed5e730a4466ab9186e18a in / 
# Fri, 12 Nov 2021 16:49:44 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 18:52:08 GMT
ARG VAULT_VERSION=1.9.2
# Wed, 22 Dec 2021 18:52:10 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 18:52:33 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 18:52:36 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 18:52:36 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 18:52:37 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 18:52:37 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 18:52:38 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 18:52:39 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 18:52:39 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:56afcfda5d78cc243287acbaad250c5e8c0f47aae620dd7c51985b0d3c9b2728`  
		Last Modified: Fri, 12 Nov 2021 16:51:32 GMT  
		Size: 2.6 MB (2635392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5fbd7bbaabf55cbd282ff7af64151efb458e0edee017c68d7bdf7766677e4e`  
		Last Modified: Wed, 22 Dec 2021 18:54:39 GMT  
		Size: 1.3 KB (1272 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05e9009a848717349f1d6242a89736d2b8073aa576394471f6aa24d964989fa3`  
		Last Modified: Wed, 22 Dec 2021 18:55:11 GMT  
		Size: 63.7 MB (63657167 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51995fc39f8fc00b85e75f5783bfaf923f5b06eefedadfb2adb76b66abe3777`  
		Last Modified: Wed, 22 Dec 2021 18:54:39 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:021ac818a2ef8ca123fcea90c7a99d831184f6304756725821e2df1dd7f3fc15`  
		Last Modified: Wed, 22 Dec 2021 18:54:38 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:a0a2220c6a23c21de8f2d0e5f77dc9ebc13275b5701c63e29c8e2a5489d993c3
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.0 MB (68037636 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e8499333f487fe90ab525d89fa43bf90adf8a35faac7ff2310a7c18ad7df3111`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:39:58 GMT
ADD file:400c0466b29ccad54e0f6c0acef22542992828678c96693ef1f9f4d0551935d8 in / 
# Fri, 12 Nov 2021 16:39:58 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 20:33:34 GMT
ARG VAULT_VERSION=1.9.2
# Wed, 22 Dec 2021 20:33:35 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 20:33:45 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 20:33:46 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 20:33:47 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 20:33:48 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 20:33:49 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 20:33:51 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 20:33:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 20:33:52 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:be307f383ecc62b27a29b599c3fc9d3129693a798e7fcce614f09174cfe2d354`  
		Last Modified: Fri, 12 Nov 2021 16:40:59 GMT  
		Size: 2.7 MB (2717700 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d29cd82552317e13f3a0054fca119ff706150dda8729d6589efe4c4765d77c21`  
		Last Modified: Wed, 22 Dec 2021 20:36:11 GMT  
		Size: 1.2 KB (1241 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d34d78dbd99bfed725c39afb795ec1fc1cdf594b6ff131c23bb935631608b175`  
		Last Modified: Wed, 22 Dec 2021 20:36:20 GMT  
		Size: 65.3 MB (65316720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:05a70fd74408902fa7157c49cfb1f48ec79d7f3b7be57e95525275c480ccfe73`  
		Last Modified: Wed, 22 Dec 2021 20:36:11 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ab137c020ad06a85a7f54d082fd711bcee0e4709847e4c38aa23eeaf241ab56`  
		Last Modified: Wed, 22 Dec 2021 20:36:11 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:4d487e3d65910ec32f0dde45c570113467c73ba52feb45f6a2d2040bf17a6a2a
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.3 MB (69318144 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d8a6ad23000600034347b2e05570777e3ed95c69bde23d86ba31abbe87de2299`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Fri, 12 Nov 2021 16:38:42 GMT
ADD file:403428c2903dd9dea10d069185873cb2c2c3149c553797807c69f22aa3d12fe3 in / 
# Fri, 12 Nov 2021 16:38:42 GMT
CMD ["/bin/sh"]
# Wed, 22 Dec 2021 20:51:01 GMT
ARG VAULT_VERSION=1.9.2
# Wed, 22 Dec 2021 20:51:04 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN addgroup vault &&     adduser -S -G vault vault
# Wed, 22 Dec 2021 20:51:20 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Wed, 22 Dec 2021 20:51:23 GMT
# ARGS: VAULT_VERSION=1.9.2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Wed, 22 Dec 2021 20:51:23 GMT
VOLUME [/vault/logs]
# Wed, 22 Dec 2021 20:51:24 GMT
VOLUME [/vault/file]
# Wed, 22 Dec 2021 20:51:24 GMT
EXPOSE 8200
# Wed, 22 Dec 2021 20:51:25 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Wed, 22 Dec 2021 20:51:26 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Wed, 22 Dec 2021 20:51:26 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:5420e0d28c84ecb16748cb90cc6acf8e2a81dab10cb1f674f3eee8533e53c62a`  
		Last Modified: Fri, 12 Nov 2021 16:39:36 GMT  
		Size: 2.8 MB (2830948 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:82e32432e839d9410dbf95acf62b3b3ee7c59d82d456fe23ee022cb11b6d56ce`  
		Last Modified: Wed, 22 Dec 2021 20:52:54 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c892bcdaac8c4aff93adfeb21a91b79e178664e79961b1805d5a935272da86f6`  
		Last Modified: Wed, 22 Dec 2021 20:53:08 GMT  
		Size: 66.5 MB (66483915 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6252140138ca5729ca2d033d267a3b01ae43ea862d21c5ed66bd2f1b615dc8cf`  
		Last Modified: Wed, 22 Dec 2021 20:52:54 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:966e79a98d455d952534442339429acb2459d3aa0d391ee39eff0a361c454d81`  
		Last Modified: Wed, 22 Dec 2021 20:52:54 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
