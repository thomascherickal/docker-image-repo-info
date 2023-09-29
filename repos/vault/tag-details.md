<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.11.11`](#vault11111)
-	[`vault:1.12.7`](#vault1127)
-	[`vault:1.13.3`](#vault1133)

## `vault:1.11.11`

```console
$ docker pull vault@sha256:242c24a6056f91dff42adc4f101d858ffb5580419e3c87001de50deab058568e
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.11.11` - linux; amd64

```console
$ docker pull vault@sha256:a23439e085e4c50067bdb6aa40b7f9f1cf16fc01e25fdfdb998ff62bebb92986
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.8 MB (81824306 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dd85824e359d4e41493ed08e2823b892d6375af97b24402ac56f221afeb65c25`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:07:06 GMT
ARG VAULT_VERSION=1.11.11
# Fri, 29 Sep 2023 00:07:06 GMT
# ARGS: VAULT_VERSION=1.11.11
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 29 Sep 2023 00:07:14 GMT
# ARGS: VAULT_VERSION=1.11.11
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 29 Sep 2023 00:07:15 GMT
# ARGS: VAULT_VERSION=1.11.11
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 29 Sep 2023 00:07:15 GMT
VOLUME [/vault/logs]
# Fri, 29 Sep 2023 00:07:15 GMT
VOLUME [/vault/file]
# Fri, 29 Sep 2023 00:07:15 GMT
EXPOSE 8200
# Fri, 29 Sep 2023 00:07:15 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 29 Sep 2023 00:07:15 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 00:07:15 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf2c9ab0ded498575f799a79107c1c80e28b1a4392b3d2559908df8d42ca4bfb`  
		Last Modified: Fri, 29 Sep 2023 00:07:59 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92493ca771cec79212603df7fff2364c0292dd40e7dc37d48c467b8f8bfd1a74`  
		Last Modified: Fri, 29 Sep 2023 00:08:09 GMT  
		Size: 78.4 MB (78419071 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5695a5b0b8e124c51c179f7c76b6130199f10b745b9c8f563f17d57cb1f85638`  
		Last Modified: Fri, 29 Sep 2023 00:07:59 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9c06141266126e408e01e2ac36e9de1ae0b1354523195fcdc8802dbb669f5d87`  
		Last Modified: Fri, 29 Sep 2023 00:07:59 GMT  
		Size: 1.8 KB (1813 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.11.11` - linux; arm variant v6

```console
$ docker pull vault@sha256:e7973c260045b113adf884d32bb942e818ef27f75bb74604a834d592a04dd556
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **76.9 MB (76870590 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a47a370590fc8aa4c7448df2c2c66eae103a18631482e37137791a0c77fdf21b`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:57:46 GMT
ARG VAULT_VERSION=1.11.11
# Fri, 29 Sep 2023 01:57:46 GMT
# ARGS: VAULT_VERSION=1.11.11
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 29 Sep 2023 01:57:57 GMT
# ARGS: VAULT_VERSION=1.11.11
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 29 Sep 2023 01:57:58 GMT
# ARGS: VAULT_VERSION=1.11.11
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 29 Sep 2023 01:57:58 GMT
VOLUME [/vault/logs]
# Fri, 29 Sep 2023 01:57:58 GMT
VOLUME [/vault/file]
# Fri, 29 Sep 2023 01:57:58 GMT
EXPOSE 8200
# Fri, 29 Sep 2023 01:57:58 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 29 Sep 2023 01:57:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 01:57:59 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:22c7fa7235063d68881b168b501adcaebbbc6a78ae11df51d150094e574806b3`  
		Last Modified: Fri, 29 Sep 2023 01:58:48 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe975f0f31dee79a309bc61f9e8dc22535805390205dda0f3c5116c5f99a83a6`  
		Last Modified: Fri, 29 Sep 2023 01:58:57 GMT  
		Size: 73.7 MB (73722030 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28a6d8842c64149dd56a4dacb482335e29e930b2eea20ce90f59bb15d6bfcdfe`  
		Last Modified: Fri, 29 Sep 2023 01:58:48 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f6277545c26de7686f8bc93b09f4426460b212181dd6412c83db5fdbd57cc46b`  
		Last Modified: Fri, 29 Sep 2023 01:58:48 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.11.11` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:23433d8b7d49004c0fb4a7d59c164610877611a3560448e4d4af7f6fedcb6d17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **77.1 MB (77144674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f9bafb985c98b1e09d718b6580e46f792641a2abffdb5fa556efafba4b75a1df`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:06:00 GMT
ARG VAULT_VERSION=1.11.11
# Fri, 29 Sep 2023 01:06:01 GMT
# ARGS: VAULT_VERSION=1.11.11
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 29 Sep 2023 01:06:08 GMT
# ARGS: VAULT_VERSION=1.11.11
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 29 Sep 2023 01:06:09 GMT
# ARGS: VAULT_VERSION=1.11.11
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 29 Sep 2023 01:06:09 GMT
VOLUME [/vault/logs]
# Fri, 29 Sep 2023 01:06:10 GMT
VOLUME [/vault/file]
# Fri, 29 Sep 2023 01:06:10 GMT
EXPOSE 8200
# Fri, 29 Sep 2023 01:06:10 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 29 Sep 2023 01:06:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 01:06:10 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a15382dd6421fe511db3a8e375bd7dd12d97089fb8efcc860b3c4ea297c1bae6`  
		Last Modified: Fri, 29 Sep 2023 01:06:53 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b86cee4bacf3ccd7a45497606a0f8714a8f9dc4a702d5aa1497fe3f147d0b55d`  
		Last Modified: Fri, 29 Sep 2023 01:07:01 GMT  
		Size: 73.8 MB (73809577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ae2004fbf049b83fb468012be1c1f62836a7fc72fc0db7cd95a82b5688376f26`  
		Last Modified: Fri, 29 Sep 2023 01:06:53 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:40c7fbf31f597c8c984df08176423a33ab5ae7df5b752fed7c16dfac6c54dca0`  
		Last Modified: Fri, 29 Sep 2023 01:06:53 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.11.11` - linux; 386

```console
$ docker pull vault@sha256:ce680c4922336c8e97f7fcd315645d1eb7ffbb42a83bf06cfcbe096e4d982ea5
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **78.5 MB (78457993 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a17d0eae8f4e29a945769473d6524958215fa478338215c67650b3038da04df9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 22:32:10 GMT
ARG VAULT_VERSION=1.11.11
# Tue, 08 Aug 2023 22:32:10 GMT
# ARGS: VAULT_VERSION=1.11.11
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 08 Aug 2023 22:32:22 GMT
# ARGS: VAULT_VERSION=1.11.11
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 08 Aug 2023 22:32:23 GMT
# ARGS: VAULT_VERSION=1.11.11
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 08 Aug 2023 22:32:23 GMT
VOLUME [/vault/logs]
# Tue, 08 Aug 2023 22:32:23 GMT
VOLUME [/vault/file]
# Tue, 08 Aug 2023 22:32:23 GMT
EXPOSE 8200
# Tue, 08 Aug 2023 22:32:24 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 08 Aug 2023 22:32:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 22:32:24 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78432155bee69bdecb1efdad9ade62fb81c3beae5a600d1a1503ead3013ade0f`  
		Last Modified: Tue, 08 Aug 2023 22:33:11 GMT  
		Size: 1.3 KB (1267 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69f87d16f57c7acbf968d12685494f576980434cfd9aee05709380946fb379be`  
		Last Modified: Tue, 08 Aug 2023 22:33:23 GMT  
		Size: 75.2 MB (75219585 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29eb17d89eebe793cdf44310e2986c8e3ac92b604f886f4e004910596c3233af`  
		Last Modified: Tue, 08 Aug 2023 22:33:11 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f058d67e13ff2c9f62b95ec4a3050f4d59008cf79d88c35887f312250f6f5c77`  
		Last Modified: Tue, 08 Aug 2023 22:33:11 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.12.7`

```console
$ docker pull vault@sha256:2731960b5a2bba7dcc10d098505f023c9fabac0ae9918e56bd425c35061d0320
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.12.7` - linux; amd64

```console
$ docker pull vault@sha256:515f333eb10b95d9fa27a3d318f017541829e315dbf3b515309835706f821131
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **86.6 MB (86570224 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08fc0d6f8f6d0aaac20ae5b75374e5b82f09270311945ae986d3719682e5cfa8`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:06:51 GMT
ARG VAULT_VERSION=1.12.7
# Fri, 29 Sep 2023 00:06:52 GMT
# ARGS: VAULT_VERSION=1.12.7
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 29 Sep 2023 00:07:00 GMT
# ARGS: VAULT_VERSION=1.12.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 29 Sep 2023 00:07:01 GMT
# ARGS: VAULT_VERSION=1.12.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 29 Sep 2023 00:07:01 GMT
VOLUME [/vault/logs]
# Fri, 29 Sep 2023 00:07:01 GMT
VOLUME [/vault/file]
# Fri, 29 Sep 2023 00:07:01 GMT
EXPOSE 8200
# Fri, 29 Sep 2023 00:07:01 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 29 Sep 2023 00:07:01 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 00:07:01 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e57ce1274ceb300782691e4a9af2c963d665e1463760085bdfaf6de26e80a47b`  
		Last Modified: Fri, 29 Sep 2023 00:07:43 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6366ea4566160a176342530fc9951b055f855a139aeb25a6f54f41df7350b22`  
		Last Modified: Fri, 29 Sep 2023 00:07:53 GMT  
		Size: 83.2 MB (83164989 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e6cc4e80bac95e7cf32632d02b9d7127941929eee8d4bd6425204098d9ab02cf`  
		Last Modified: Fri, 29 Sep 2023 00:07:43 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b59a4bc4e88ec41daeef117fbc6a59732dcebba5bb8c7bd83c2f85e9af1af75`  
		Last Modified: Fri, 29 Sep 2023 00:07:43 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.12.7` - linux; arm variant v6

```console
$ docker pull vault@sha256:f29f529fcb04503ae790de5121878b921397a339662d03f10db47d53a9e218af
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.2 MB (81228666 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2ab2a24120600230f389841bc0af4ce1f7a76df076db36f56b16b4900cc8dfbd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:57:29 GMT
ARG VAULT_VERSION=1.12.7
# Fri, 29 Sep 2023 01:57:30 GMT
# ARGS: VAULT_VERSION=1.12.7
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 29 Sep 2023 01:57:41 GMT
# ARGS: VAULT_VERSION=1.12.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 29 Sep 2023 01:57:42 GMT
# ARGS: VAULT_VERSION=1.12.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 29 Sep 2023 01:57:42 GMT
VOLUME [/vault/logs]
# Fri, 29 Sep 2023 01:57:43 GMT
VOLUME [/vault/file]
# Fri, 29 Sep 2023 01:57:43 GMT
EXPOSE 8200
# Fri, 29 Sep 2023 01:57:43 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 29 Sep 2023 01:57:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 01:57:43 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec4efdea16aca03bfc76986828f72f6e69aaa71948d4c5f9cb23dd63d1380dc6`  
		Last Modified: Fri, 29 Sep 2023 01:58:31 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad0a8dffb36e1a55c36f27435b1e1bbf2a5e4b77e14e3e75abae946abfd1c13b`  
		Last Modified: Fri, 29 Sep 2023 01:58:41 GMT  
		Size: 78.1 MB (78080106 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52eae186e3330e152b3c47e66bae975d5ccbe2fbdcc7aa9a843dbe02f1095c48`  
		Last Modified: Fri, 29 Sep 2023 01:58:31 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eadaf14f3152d0a5fc7f402b622c1df914e2086255e0874e555fd51ee7e8d564`  
		Last Modified: Fri, 29 Sep 2023 01:58:31 GMT  
		Size: 1.8 KB (1811 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.12.7` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:85cdb90c57ae7fbd1f5ae2ce1f00be40e66ad58bbf729adeecdd62abc8815756
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **81.7 MB (81675479 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:32a043eb145bee8b91387c878e5fbb2f47ddbdcda0a10307742e0070de6275b9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:05:47 GMT
ARG VAULT_VERSION=1.12.7
# Fri, 29 Sep 2023 01:05:47 GMT
# ARGS: VAULT_VERSION=1.12.7
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 29 Sep 2023 01:05:56 GMT
# ARGS: VAULT_VERSION=1.12.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 29 Sep 2023 01:05:58 GMT
# ARGS: VAULT_VERSION=1.12.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 29 Sep 2023 01:05:58 GMT
VOLUME [/vault/logs]
# Fri, 29 Sep 2023 01:05:58 GMT
VOLUME [/vault/file]
# Fri, 29 Sep 2023 01:05:58 GMT
EXPOSE 8200
# Fri, 29 Sep 2023 01:05:58 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 29 Sep 2023 01:05:58 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 01:05:58 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:022135de7e7750b45f0d28446534cc81acded7d25a7db0f5ddd3bebf2a7e185a`  
		Last Modified: Fri, 29 Sep 2023 01:06:34 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:572da0e7510376f27208631f9f0f591bffba1df6c1b2a12e4679338418727ea6`  
		Last Modified: Fri, 29 Sep 2023 01:06:46 GMT  
		Size: 78.3 MB (78340379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:94251d879212f40ef3a2f954ecf3d1b9edcc5d342d007f0a9220a494eb893322`  
		Last Modified: Fri, 29 Sep 2023 01:06:34 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a5eb3af34090b40d93db500771ce4e87d429797bbc40678dcefd4d51070ff5ab`  
		Last Modified: Fri, 29 Sep 2023 01:06:34 GMT  
		Size: 1.8 KB (1812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.12.7` - linux; 386

```console
$ docker pull vault@sha256:1e646b0fc35ca5fadf605e6a943df59c78c1f374cc681574c12470f7ecf2fdeb
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **82.8 MB (82842079 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:7cc054fc4559095c0d96d2a0f9d99045464d2ae6979ce12bd58af2173b41c502`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 22:31:54 GMT
ARG VAULT_VERSION=1.12.7
# Tue, 08 Aug 2023 22:31:54 GMT
# ARGS: VAULT_VERSION=1.12.7
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 08 Aug 2023 22:32:06 GMT
# ARGS: VAULT_VERSION=1.12.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 08 Aug 2023 22:32:07 GMT
# ARGS: VAULT_VERSION=1.12.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 08 Aug 2023 22:32:08 GMT
VOLUME [/vault/logs]
# Tue, 08 Aug 2023 22:32:08 GMT
VOLUME [/vault/file]
# Tue, 08 Aug 2023 22:32:08 GMT
EXPOSE 8200
# Tue, 08 Aug 2023 22:32:08 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 08 Aug 2023 22:32:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 22:32:08 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f16bfe3cbbd55209f3f2097992a7d28016c7a36a211fc28aed97a00da42300f6`  
		Last Modified: Tue, 08 Aug 2023 22:32:53 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f2eb5a9d42b224a0d4baeabc30826aa769763d8e890df06744b2dd87d8593f44`  
		Last Modified: Tue, 08 Aug 2023 22:33:05 GMT  
		Size: 79.6 MB (79603664 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69900e1ee56d826803c24d494c8a80ceecd7c57c343f7f297c48e83a89d64153`  
		Last Modified: Tue, 08 Aug 2023 22:32:53 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1930cb953612fbff81f510170d60691ba8587a597bf60e5789f6421bd1c1ca5e`  
		Last Modified: Tue, 08 Aug 2023 22:32:53 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.13.3`

```console
$ docker pull vault@sha256:27e0aaf2e4582dd98d0114217eba3f757641792cc2b7213edfe070fbc88d47cf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.13.3` - linux; amd64

```console
$ docker pull vault@sha256:d639ad7bebc3ddcbc88f529b4f8baa85743a9a24248c4285d958f90f56682836
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **97.6 MB (97610963 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6d1fcd1a47eb84358f17a6918352cdf576f606d9fc9d36e8d13d9c9315ad89f9`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 28 Sep 2023 21:19:27 GMT
ADD file:756183bba9c7f4593c2b216e98e4208b9163c4c962ea0837ef88bd917609d001 in / 
# Thu, 28 Sep 2023 21:19:27 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 00:06:37 GMT
ARG VAULT_VERSION=1.13.3
# Fri, 29 Sep 2023 00:06:37 GMT
# ARGS: VAULT_VERSION=1.13.3
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 29 Sep 2023 00:06:46 GMT
# ARGS: VAULT_VERSION=1.13.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 29 Sep 2023 00:06:47 GMT
# ARGS: VAULT_VERSION=1.13.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 29 Sep 2023 00:06:47 GMT
VOLUME [/vault/logs]
# Fri, 29 Sep 2023 00:06:47 GMT
VOLUME [/vault/file]
# Fri, 29 Sep 2023 00:06:47 GMT
EXPOSE 8200
# Fri, 29 Sep 2023 00:06:47 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 29 Sep 2023 00:06:47 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 00:06:47 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:96526aa774ef0126ad0fe9e9a95764c5fc37f409ab9e97021e7b4775d82bf6fa`  
		Last Modified: Thu, 28 Sep 2023 21:22:06 GMT  
		Size: 3.4 MB (3401967 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bb96b81cd1906c01728b67a48938978114de18094c6bc88ae674b58bf343f853`  
		Last Modified: Fri, 29 Sep 2023 00:07:24 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29f5d86fa0f2da37d5dc8672c53fe2d4895073dcec759fdeed587f279afcbe83`  
		Last Modified: Fri, 29 Sep 2023 00:07:37 GMT  
		Size: 94.2 MB (94205728 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c0e14a2dc26dfa04dbee8d5ed1efd8f8de4df2da04a915a4e376d8a296ef26`  
		Last Modified: Fri, 29 Sep 2023 00:07:24 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28703b214f38bf539e7163a2bfeaa31e5cd42d0e84f7262ecd8e1ecc0b07d4a9`  
		Last Modified: Fri, 29 Sep 2023 00:07:24 GMT  
		Size: 1.8 KB (1810 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.13.3` - linux; arm variant v6

```console
$ docker pull vault@sha256:dce6bc2058f24ebe856f979e90d51455190f6dec90997c6fe6ebe6f3d862ee2d
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **91.6 MB (91637912 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:08fb75d3751a2b02dd7da8076d2d1bdd26d12c339cc0043fdeb8a12c80a335ce`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 28 Sep 2023 20:49:16 GMT
ADD file:2222b03381ff0fce22edd647f5c60529ec6a72202f8d3cb1d6e4648ebcd19a1e in / 
# Thu, 28 Sep 2023 20:49:16 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:57:10 GMT
ARG VAULT_VERSION=1.13.3
# Fri, 29 Sep 2023 01:57:10 GMT
# ARGS: VAULT_VERSION=1.13.3
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 29 Sep 2023 01:57:23 GMT
# ARGS: VAULT_VERSION=1.13.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 29 Sep 2023 01:57:24 GMT
# ARGS: VAULT_VERSION=1.13.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 29 Sep 2023 01:57:24 GMT
VOLUME [/vault/logs]
# Fri, 29 Sep 2023 01:57:25 GMT
VOLUME [/vault/file]
# Fri, 29 Sep 2023 01:57:25 GMT
EXPOSE 8200
# Fri, 29 Sep 2023 01:57:25 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 29 Sep 2023 01:57:25 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 01:57:25 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:91cb83b91ee16f1ee0d588fccef56ab5dbb5689a64e5373caf33d7e4fe52ceb4`  
		Last Modified: Thu, 28 Sep 2023 20:51:25 GMT  
		Size: 3.1 MB (3145291 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eac6a25beda6aa37c8e0e9b94eef61613117336b1e9343f63c8c91be33db6c5f`  
		Last Modified: Fri, 29 Sep 2023 01:58:09 GMT  
		Size: 1.3 KB (1271 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a163e87d25ac119df14f7aebf18f8a2563e0350512f9beadf3ef71dea8e36b93`  
		Last Modified: Fri, 29 Sep 2023 01:58:20 GMT  
		Size: 88.5 MB (88489350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ee471bf294bc6e73af7de9a11d9aa1daac0f3387917f1b4d19162d1e27efdab2`  
		Last Modified: Fri, 29 Sep 2023 01:58:09 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea115b4b7564a8fecec31b469c874e616be2c988325895539b35eac108d0d265`  
		Last Modified: Fri, 29 Sep 2023 01:58:09 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.13.3` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:63359fc91e5e6e4b6c6208223575c935ce64cb906735b7790efeadb0a8392d17
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **92.2 MB (92163467 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:80d4968b1bbe49f83ae54121fc17499c4bca0fe3a6a2be39b5466c2ca46b3014`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 28 Sep 2023 20:39:33 GMT
ADD file:ff3112828967e8004a3264d7ece3f81c88e6a1d44d360b9b5613caab15b41717 in / 
# Thu, 28 Sep 2023 20:39:34 GMT
CMD ["/bin/sh"]
# Fri, 29 Sep 2023 01:05:30 GMT
ARG VAULT_VERSION=1.13.3
# Fri, 29 Sep 2023 01:05:31 GMT
# ARGS: VAULT_VERSION=1.13.3
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 29 Sep 2023 01:05:41 GMT
# ARGS: VAULT_VERSION=1.13.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 29 Sep 2023 01:05:43 GMT
# ARGS: VAULT_VERSION=1.13.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 29 Sep 2023 01:05:43 GMT
VOLUME [/vault/logs]
# Fri, 29 Sep 2023 01:05:43 GMT
VOLUME [/vault/file]
# Fri, 29 Sep 2023 01:05:43 GMT
EXPOSE 8200
# Fri, 29 Sep 2023 01:05:43 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 29 Sep 2023 01:05:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 29 Sep 2023 01:05:44 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:579b34f0a95bb83b3acd6b3249ddc52c3d80f5c84b13c944e9e324feb86dd329`  
		Last Modified: Thu, 28 Sep 2023 20:40:08 GMT  
		Size: 3.3 MB (3331831 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:458f409a123a9e8a3c302bdbf14832dbd6ec06d0eb03ecba8bae312f40adb4d2`  
		Last Modified: Fri, 29 Sep 2023 01:06:19 GMT  
		Size: 1.3 KB (1270 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad5986c31e0fea43702ab50de7b168c4d4f4640f4ff4d151c21a0a9ced7d53e`  
		Last Modified: Fri, 29 Sep 2023 01:06:27 GMT  
		Size: 88.8 MB (88828365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b698e9340015199b16b8af94e98b4f889cc2325ce9cd26612493ac3a8a80ee7`  
		Last Modified: Fri, 29 Sep 2023 01:06:19 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:008f12083f964359307303a74394ff4e1063e69430f5bde46df89a777b1edfcf`  
		Last Modified: Fri, 29 Sep 2023 01:06:19 GMT  
		Size: 1.8 KB (1814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.13.3` - linux; 386

```console
$ docker pull vault@sha256:3b0be5ed26c804a59b66991f429f59ed0e786a9b6a89662dd4e4720b0d4c8876
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **93.3 MB (93257289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8247e8f3f2cfca6802846969de74f3fd2f686c85f789b17e90784aa2d0cb4b37`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Mon, 07 Aug 2023 19:38:26 GMT
ADD file:4b33c52e11b19fde30197c62ead0b77bde28d34edaa08346a5302cd892d3cebe in / 
# Mon, 07 Aug 2023 19:38:27 GMT
CMD ["/bin/sh"]
# Tue, 08 Aug 2023 22:31:37 GMT
ARG VAULT_VERSION=1.13.3
# Tue, 08 Aug 2023 22:31:38 GMT
# ARGS: VAULT_VERSION=1.13.3
RUN addgroup vault &&     adduser -S -G vault vault
# Tue, 08 Aug 2023 22:31:49 GMT
# ARGS: VAULT_VERSION=1.13.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=C874011F0AB405110D02105534365D9472D7468F;     found='';     for server in         hkps://keys.openpgp.org         hkps://keyserver.ubuntu.com         hkps://pgp.mit.edu     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /tmp/build vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cp /tmp/build/vault /bin/vault &&     if [ -f /tmp/build/EULA.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/EULA.txt /usr/share/doc/vault/EULA.txt; fi &&     if [ -f /tmp/build/TermsOfEvaluation.txt ]; then mkdir -p /usr/share/doc/vault; mv /tmp/build/TermsOfEvaluation.txt /usr/share/doc/vault/TermsOfEvaluation.txt; fi &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Tue, 08 Aug 2023 22:31:50 GMT
# ARGS: VAULT_VERSION=1.13.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Tue, 08 Aug 2023 22:31:50 GMT
VOLUME [/vault/logs]
# Tue, 08 Aug 2023 22:31:50 GMT
VOLUME [/vault/file]
# Tue, 08 Aug 2023 22:31:50 GMT
EXPOSE 8200
# Tue, 08 Aug 2023 22:31:51 GMT
COPY file:284725e82dfade67c8b2092585f70a151b8782d83106082a5b4852b996b7e550 in /usr/local/bin/docker-entrypoint.sh 
# Tue, 08 Aug 2023 22:31:51 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Tue, 08 Aug 2023 22:31:51 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:95dc695758361a4038a2d9026959d72e1f531114edb0341be7ce47d912ef069e`  
		Last Modified: Mon, 07 Aug 2023 19:38:56 GMT  
		Size: 3.2 MB (3235144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:364df086ffbef3c77794150521f7047346239d4c91fe1e708831a4e5228fb4c8`  
		Last Modified: Tue, 08 Aug 2023 22:32:34 GMT  
		Size: 1.3 KB (1269 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bf07ad172204b23bf5cac2621f4f81ea847b615983ebf08f1027815cf66b919`  
		Last Modified: Tue, 08 Aug 2023 22:32:47 GMT  
		Size: 90.0 MB (90018882 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9a64676d5c3b49dc2e26606cb55ce22a9dacde41bf5404dadccbcdcba2ef49b7`  
		Last Modified: Tue, 08 Aug 2023 22:32:33 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61b41fe279b5833f91f809955d3a1e29ba45f23fc554182bd05dd45f0144dd22`  
		Last Modified: Tue, 08 Aug 2023 22:32:33 GMT  
		Size: 1.8 KB (1807 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
