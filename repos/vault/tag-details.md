<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.3.4`](#vault134)
-	[`vault:1.4.0-rc1`](#vault140-rc1)
-	[`vault:latest`](#vaultlatest)

## `vault:1.3.4`

```console
$ docker pull vault@sha256:fca20e29378b5d7917f14395a54d045ef8d81cd40ecf2c4a1da44e629ecf9e34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.3.4` - linux; amd64

```console
$ docker pull vault@sha256:765b4b615cbbc6cf4103c18ae359d65a98ef2e40a7c58feb7285885606a247cf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51653805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2486a1b22ec0f7b7fbc2c831d172e5687d744a55c2b82bac5ef369e16f8a29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 20 Mar 2020 18:21:49 GMT
ARG VAULT_VERSION=1.3.4
# Fri, 20 Mar 2020 18:21:50 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 20 Mar 2020 18:21:55 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 20 Mar 2020 18:21:55 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 20 Mar 2020 18:21:56 GMT
VOLUME [/vault/logs]
# Fri, 20 Mar 2020 18:21:56 GMT
VOLUME [/vault/file]
# Fri, 20 Mar 2020 18:21:56 GMT
EXPOSE 8200
# Fri, 20 Mar 2020 18:21:56 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 20 Mar 2020 18:21:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 18:21:56 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21bb3058b0b57cd5066db6494c6b9a8552526ed740beda8eda9c7cfbde45d512`  
		Last Modified: Fri, 20 Mar 2020 18:22:15 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feaca4738ab0020b3e873aa578da36eb224f3ef05e43e85122a265022ef8b90`  
		Last Modified: Fri, 20 Mar 2020 18:22:23 GMT  
		Size: 48.9 MB (48863609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3660910fc75eae4c5a40912a22849400af0a893334ed9404439f6ef79d2eb2`  
		Last Modified: Fri, 20 Mar 2020 18:22:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18309fece480daaca4b8b52069639db90a603cf497a2e9a8ce0115da73523eb`  
		Last Modified: Fri, 20 Mar 2020 18:22:15 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.3.4` - linux; arm variant v6

```console
$ docker pull vault@sha256:6aae627b40baa86d99f1d062a1409ce350dc15744046d117bee8846c80f2b594
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48655160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8a4bd49ebd4b13fb9e3ea8da0fcc5a2d7dacfa77358a6920b29d81f6b1ae8cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Fri, 20 Mar 2020 17:49:36 GMT
ARG VAULT_VERSION=1.3.4
# Fri, 20 Mar 2020 17:49:38 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 20 Mar 2020 17:49:48 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 20 Mar 2020 17:49:50 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 20 Mar 2020 17:49:50 GMT
VOLUME [/vault/logs]
# Fri, 20 Mar 2020 17:49:51 GMT
VOLUME [/vault/file]
# Fri, 20 Mar 2020 17:49:51 GMT
EXPOSE 8200
# Fri, 20 Mar 2020 17:49:52 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 20 Mar 2020 17:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 17:49:54 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad58a6bae42e65d7f7209ad5e7a797e5ec88f41f7e04648b201a33086dd8a30`  
		Last Modified: Fri, 20 Mar 2020 17:50:26 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b62737b423cdf152ab834afc431527f4528fe66413e0cd6b2f903eabb6d2d1`  
		Last Modified: Fri, 20 Mar 2020 17:50:40 GMT  
		Size: 46.1 MB (46080457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d214108e4978958534ca440fb45f2a8a1bb3e369143a3295f7bc4fd207a4bed`  
		Last Modified: Fri, 20 Mar 2020 17:50:26 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9e96a5f8158485ff78f6b1f474f15fcdfe1617e910e0befcfff3f3d41a9c26`  
		Last Modified: Fri, 20 Mar 2020 17:50:26 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.3.4` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:7fa8c11454f3d921f5326b33bae85d50f58e13698ff01895d36bbbc7fa82659b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48705749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5095c0a907c9f3a9e09d470cc180292d3e2f908f552db2bde38cde92fa410b8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Fri, 20 Mar 2020 17:40:56 GMT
ARG VAULT_VERSION=1.3.4
# Fri, 20 Mar 2020 17:40:58 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 20 Mar 2020 17:41:06 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 20 Mar 2020 17:41:09 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 20 Mar 2020 17:41:09 GMT
VOLUME [/vault/logs]
# Fri, 20 Mar 2020 17:41:10 GMT
VOLUME [/vault/file]
# Fri, 20 Mar 2020 17:41:11 GMT
EXPOSE 8200
# Fri, 20 Mar 2020 17:41:11 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 20 Mar 2020 17:41:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 17:41:12 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46807f3bbe9cd93e3a5f4568435b86c3653c53dd511a05dad0116c2a6ecf785b`  
		Last Modified: Fri, 20 Mar 2020 17:41:42 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4d8d2311beb1df19d586a93f75f03945795ad40d8b59218a333f52f9d9be72`  
		Last Modified: Fri, 20 Mar 2020 17:41:54 GMT  
		Size: 46.0 MB (45984720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955df15b21eb94c11d7658c8047b361c6a2aaa85d6b545b5ab9c162bea5fbd02`  
		Last Modified: Fri, 20 Mar 2020 17:41:42 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ee842172143d692f9f8edfff917c4c1373545454ce72ae38eee90ccdff0996`  
		Last Modified: Fri, 20 Mar 2020 17:41:42 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.3.4` - linux; 386

```console
$ docker pull vault@sha256:5508339488538befe018ed433452e0c501329b228c5cc5714d099df1e7a0f807
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50111543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64897c105b9e1b305ecaa4443dffac9f398eee8fcae6796a65a82d7b16326f30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 20 Mar 2020 17:38:55 GMT
ARG VAULT_VERSION=1.3.4
# Fri, 20 Mar 2020 17:38:56 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 20 Mar 2020 17:39:02 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 20 Mar 2020 17:39:03 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 20 Mar 2020 17:39:03 GMT
VOLUME [/vault/logs]
# Fri, 20 Mar 2020 17:39:03 GMT
VOLUME [/vault/file]
# Fri, 20 Mar 2020 17:39:03 GMT
EXPOSE 8200
# Fri, 20 Mar 2020 17:39:04 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 20 Mar 2020 17:39:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 17:39:04 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195ddf817abf9b727a89d330e4c1749a26daa4f739a732b1f338eb5b3e6c2c47`  
		Last Modified: Fri, 20 Mar 2020 17:39:25 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e7ed4e25c12c477182ca7df0f8dbe33a2a0d5e2d384b7b71ca2c042e7a8ce0`  
		Last Modified: Fri, 20 Mar 2020 17:39:33 GMT  
		Size: 47.3 MB (47322442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbb751b023a72b97b2d81be1897efc8b90d04b9038332d55fd4eb5891700027`  
		Last Modified: Fri, 20 Mar 2020 17:39:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9279d72ca2647322e294804e55a4964b3941eac71139401ba6c3b1b4d9e72ce8`  
		Last Modified: Fri, 20 Mar 2020 17:39:24 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.4.0-rc1`

```console
$ docker pull vault@sha256:894fcd93cf8f5f2a8b486891d59321e0321ce1c2bf0abdbd531d83761dec1160
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.4.0-rc1` - linux; amd64

```console
$ docker pull vault@sha256:0a6907e1aa2d46c9ba93493ce24d9329339d7b66ed471a878846d017c1be0ea0
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.0 MB (52030870 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:96ff50e6920e7fe204411188a7fbe1a436aa473da0706031c4649332910e5dba`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 20 Mar 2020 18:22:01 GMT
ARG VAULT_VERSION=1.4.0-rc1
# Fri, 20 Mar 2020 18:22:01 GMT
# ARGS: VAULT_VERSION=1.4.0-rc1
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 20 Mar 2020 18:22:06 GMT
# ARGS: VAULT_VERSION=1.4.0-rc1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 20 Mar 2020 18:22:07 GMT
# ARGS: VAULT_VERSION=1.4.0-rc1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 20 Mar 2020 18:22:07 GMT
VOLUME [/vault/logs]
# Fri, 20 Mar 2020 18:22:07 GMT
VOLUME [/vault/file]
# Fri, 20 Mar 2020 18:22:08 GMT
EXPOSE 8200
# Fri, 20 Mar 2020 18:22:08 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 20 Mar 2020 18:22:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 18:22:08 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c89eaad2faea335dfe24caceb235ae2804b30fd39f0400c15364e67aa4f22da`  
		Last Modified: Fri, 20 Mar 2020 18:22:28 GMT  
		Size: 1.3 KB (1262 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b1305785f97f935dca1b92c8b1a9e685d10def20a572e9a8478cc04e958c216`  
		Last Modified: Fri, 20 Mar 2020 18:22:38 GMT  
		Size: 49.2 MB (49240672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8355f8cf06e271d0bf535e6be1a58f4b7b2554fad0a7f437c05180ed27ce4383`  
		Last Modified: Fri, 20 Mar 2020 18:22:27 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dd5a5982f3c5c749be1e46feb42d7fa017d251ef814d81f47d915c2f134ac04f`  
		Last Modified: Fri, 20 Mar 2020 18:22:28 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.0-rc1` - linux; arm variant v6

```console
$ docker pull vault@sha256:21c251dace9bdc924be089c3b629c0fcd86611199cbaef1edd0b9b9bdf45a7b9
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48687990 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9c9d7a97b4a746a1719babe3d1dba5d690a2da6f9d14fe84b9decd87fa00a3e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Fri, 20 Mar 2020 17:50:01 GMT
ARG VAULT_VERSION=1.4.0-rc1
# Fri, 20 Mar 2020 17:50:03 GMT
# ARGS: VAULT_VERSION=1.4.0-rc1
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 20 Mar 2020 17:50:12 GMT
# ARGS: VAULT_VERSION=1.4.0-rc1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 20 Mar 2020 17:50:14 GMT
# ARGS: VAULT_VERSION=1.4.0-rc1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 20 Mar 2020 17:50:15 GMT
VOLUME [/vault/logs]
# Fri, 20 Mar 2020 17:50:15 GMT
VOLUME [/vault/file]
# Fri, 20 Mar 2020 17:50:16 GMT
EXPOSE 8200
# Fri, 20 Mar 2020 17:50:16 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 20 Mar 2020 17:50:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 17:50:18 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8586e0afdfddff11827b170f00f9ca5f67514a35990a0b0a509057b1b810abc8`  
		Last Modified: Fri, 20 Mar 2020 17:50:46 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f5e402ef7e274e85e12bf66e05c09192df1ad3dbd195d6a3248b8058088f3f1`  
		Last Modified: Fri, 20 Mar 2020 17:50:59 GMT  
		Size: 46.1 MB (46113284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b6f1a87f728c151a2ed62b750b4189cafb662c7dd0855deafbeb7bc28a70696`  
		Last Modified: Fri, 20 Mar 2020 17:50:46 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d8e5055100c7c4e223051f3bc738332f5ced6d3a5754b63cc76fd64ae18a2d98`  
		Last Modified: Fri, 20 Mar 2020 17:50:46 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.0-rc1` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:2a0547cc8c0406fb233c7207e6a8a69678b9112cddf59c31ba3443863848bc1b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48963221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:93ec443a717d79289f56373eca231815401fc3bf1bfdd473f2a38c0c646cd8e4`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Fri, 20 Mar 2020 17:41:20 GMT
ARG VAULT_VERSION=1.4.0-rc1
# Fri, 20 Mar 2020 17:41:22 GMT
# ARGS: VAULT_VERSION=1.4.0-rc1
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 20 Mar 2020 17:41:29 GMT
# ARGS: VAULT_VERSION=1.4.0-rc1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 20 Mar 2020 17:41:31 GMT
# ARGS: VAULT_VERSION=1.4.0-rc1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 20 Mar 2020 17:41:32 GMT
VOLUME [/vault/logs]
# Fri, 20 Mar 2020 17:41:32 GMT
VOLUME [/vault/file]
# Fri, 20 Mar 2020 17:41:33 GMT
EXPOSE 8200
# Fri, 20 Mar 2020 17:41:33 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 20 Mar 2020 17:41:34 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 17:41:35 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e20441a0238bbe5d13eb9ddcb88c1b16e2a22e72832790c235cfb4fb0119811e`  
		Last Modified: Fri, 20 Mar 2020 17:42:00 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3c6a8971c0754db6d30922ec5b8fabad7e4120c20d5c70aadf63101c51033d38`  
		Last Modified: Fri, 20 Mar 2020 17:42:12 GMT  
		Size: 46.2 MB (46242189 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c31ee8ffa13394a9a34d7a2fd7e469fdde935f53aac5661611b3e060ed848d3`  
		Last Modified: Fri, 20 Mar 2020 17:42:00 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:db0c9f985ae3407490c9c848fa12d176e259ec4c766d978a153c43d94633d384`  
		Last Modified: Fri, 20 Mar 2020 17:42:00 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.0-rc1` - linux; 386

```console
$ docker pull vault@sha256:f0e17defa5ae03d68ab846cf73ef34ed83f74cbb147836165781a840a40aeac3
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50189414 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5728ce887dbfabe9f03d1259b31e76e9878c6c7e8c179cbc581ca12f96f8eba7`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 20 Mar 2020 17:39:09 GMT
ARG VAULT_VERSION=1.4.0-rc1
# Fri, 20 Mar 2020 17:39:09 GMT
# ARGS: VAULT_VERSION=1.4.0-rc1
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 20 Mar 2020 17:39:15 GMT
# ARGS: VAULT_VERSION=1.4.0-rc1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 20 Mar 2020 17:39:16 GMT
# ARGS: VAULT_VERSION=1.4.0-rc1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 20 Mar 2020 17:39:16 GMT
VOLUME [/vault/logs]
# Fri, 20 Mar 2020 17:39:16 GMT
VOLUME [/vault/file]
# Fri, 20 Mar 2020 17:39:16 GMT
EXPOSE 8200
# Fri, 20 Mar 2020 17:39:17 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 20 Mar 2020 17:39:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 17:39:17 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31af4e79805e3a0b8f6b64526b5225dab16b4a3517d2ad08580a458de3b34b82`  
		Last Modified: Fri, 20 Mar 2020 17:39:37 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6d86096c055401e4020d1c5b930b64b50ce4e8a3f36fa8e34b97bc2cd27bf29`  
		Last Modified: Fri, 20 Mar 2020 17:39:45 GMT  
		Size: 47.4 MB (47400315 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57cba61e6600aa38166b83ccacc13d9a619aa6b5cee0db083ab536556291d07d`  
		Last Modified: Fri, 20 Mar 2020 17:39:37 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8c36819c217ddfa2ff52bc1e1b9a70d9e5d06ab9fd69532091dfc3545edf983e`  
		Last Modified: Fri, 20 Mar 2020 17:39:37 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:fca20e29378b5d7917f14395a54d045ef8d81cd40ecf2c4a1da44e629ecf9e34
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:765b4b615cbbc6cf4103c18ae359d65a98ef2e40a7c58feb7285885606a247cf
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.7 MB (51653805 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0c2486a1b22ec0f7b7fbc2c831d172e5687d744a55c2b82bac5ef369e16f8a29`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:06 GMT
ADD file:d48cac34fac385cbc1de6adfdd88300f76f9bbe346cd17e64fd834d042a98326 in / 
# Thu, 23 Jan 2020 16:53:06 GMT
CMD ["/bin/sh"]
# Fri, 20 Mar 2020 18:21:49 GMT
ARG VAULT_VERSION=1.3.4
# Fri, 20 Mar 2020 18:21:50 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 20 Mar 2020 18:21:55 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 20 Mar 2020 18:21:55 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 20 Mar 2020 18:21:56 GMT
VOLUME [/vault/logs]
# Fri, 20 Mar 2020 18:21:56 GMT
VOLUME [/vault/file]
# Fri, 20 Mar 2020 18:21:56 GMT
EXPOSE 8200
# Fri, 20 Mar 2020 18:21:56 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 20 Mar 2020 18:21:56 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 18:21:56 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:4167d3e149762ea326c26fc2fd4e36fdeb7d4e639408ad30f37b8f25ac285a98`  
		Last Modified: Thu, 23 Jan 2020 16:53:38 GMT  
		Size: 2.8 MB (2786962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:21bb3058b0b57cd5066db6494c6b9a8552526ed740beda8eda9c7cfbde45d512`  
		Last Modified: Fri, 20 Mar 2020 18:22:15 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3feaca4738ab0020b3e873aa578da36eb224f3ef05e43e85122a265022ef8b90`  
		Last Modified: Fri, 20 Mar 2020 18:22:23 GMT  
		Size: 48.9 MB (48863609 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f3660910fc75eae4c5a40912a22849400af0a893334ed9404439f6ef79d2eb2`  
		Last Modified: Fri, 20 Mar 2020 18:22:15 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f18309fece480daaca4b8b52069639db90a603cf497a2e9a8ce0115da73523eb`  
		Last Modified: Fri, 20 Mar 2020 18:22:15 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:6aae627b40baa86d99f1d062a1409ce350dc15744046d117bee8846c80f2b594
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48655160 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8a4bd49ebd4b13fb9e3ea8da0fcc5a2d7dacfa77358a6920b29d81f6b1ae8cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:53:27 GMT
ADD file:2aa80d52585a6b34b2cc5811d46965a084e50cfb8cd183f1a88b2b1bc6556e1f in / 
# Thu, 23 Jan 2020 16:53:28 GMT
CMD ["/bin/sh"]
# Fri, 20 Mar 2020 17:49:36 GMT
ARG VAULT_VERSION=1.3.4
# Fri, 20 Mar 2020 17:49:38 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 20 Mar 2020 17:49:48 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 20 Mar 2020 17:49:50 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 20 Mar 2020 17:49:50 GMT
VOLUME [/vault/logs]
# Fri, 20 Mar 2020 17:49:51 GMT
VOLUME [/vault/file]
# Fri, 20 Mar 2020 17:49:51 GMT
EXPOSE 8200
# Fri, 20 Mar 2020 17:49:52 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 20 Mar 2020 17:49:53 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 17:49:54 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:896868b7b9168cabb308702db96dc9769d10c23e20fc66f5f4abedf4c75d7642`  
		Last Modified: Thu, 23 Jan 2020 16:54:07 GMT  
		Size: 2.6 MB (2571407 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fad58a6bae42e65d7f7209ad5e7a797e5ec88f41f7e04648b201a33086dd8a30`  
		Last Modified: Fri, 20 Mar 2020 17:50:26 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:29b62737b423cdf152ab834afc431527f4528fe66413e0cd6b2f903eabb6d2d1`  
		Last Modified: Fri, 20 Mar 2020 17:50:40 GMT  
		Size: 46.1 MB (46080457 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d214108e4978958534ca440fb45f2a8a1bb3e369143a3295f7bc4fd207a4bed`  
		Last Modified: Fri, 20 Mar 2020 17:50:26 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b9e96a5f8158485ff78f6b1f474f15fcdfe1617e910e0befcfff3f3d41a9c26`  
		Last Modified: Fri, 20 Mar 2020 17:50:26 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:7fa8c11454f3d921f5326b33bae85d50f58e13698ff01895d36bbbc7fa82659b
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48705749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5095c0a907c9f3a9e09d470cc180292d3e2f908f552db2bde38cde92fa410b8a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:54:39 GMT
ADD file:bdfbd4b0dfb53eecc80bac65894d1e2fcfafb27dcf24ab019176e2c9f60b9a39 in / 
# Thu, 23 Jan 2020 16:54:40 GMT
CMD ["/bin/sh"]
# Fri, 20 Mar 2020 17:40:56 GMT
ARG VAULT_VERSION=1.3.4
# Fri, 20 Mar 2020 17:40:58 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 20 Mar 2020 17:41:06 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 20 Mar 2020 17:41:09 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 20 Mar 2020 17:41:09 GMT
VOLUME [/vault/logs]
# Fri, 20 Mar 2020 17:41:10 GMT
VOLUME [/vault/file]
# Fri, 20 Mar 2020 17:41:11 GMT
EXPOSE 8200
# Fri, 20 Mar 2020 17:41:11 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 20 Mar 2020 17:41:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 17:41:12 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:f07e4bcf42b862c240f4c00f2f7ed362d7d93ca15151de547beda593f3b669e5`  
		Last Modified: Thu, 23 Jan 2020 16:55:24 GMT  
		Size: 2.7 MB (2717732 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:46807f3bbe9cd93e3a5f4568435b86c3653c53dd511a05dad0116c2a6ecf785b`  
		Last Modified: Fri, 20 Mar 2020 17:41:42 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fd4d8d2311beb1df19d586a93f75f03945795ad40d8b59218a333f52f9d9be72`  
		Last Modified: Fri, 20 Mar 2020 17:41:54 GMT  
		Size: 46.0 MB (45984720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:955df15b21eb94c11d7658c8047b361c6a2aaa85d6b545b5ab9c162bea5fbd02`  
		Last Modified: Fri, 20 Mar 2020 17:41:42 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f3ee842172143d692f9f8edfff917c4c1373545454ce72ae38eee90ccdff0996`  
		Last Modified: Fri, 20 Mar 2020 17:41:42 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:5508339488538befe018ed433452e0c501329b228c5cc5714d099df1e7a0f807
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.1 MB (50111543 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:64897c105b9e1b305ecaa4443dffac9f398eee8fcae6796a65a82d7b16326f30`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Thu, 23 Jan 2020 16:52:57 GMT
ADD file:8c429ecc11f3cadcecc39922ce15df6b51a649929959b331fed8d1f42d722474 in / 
# Thu, 23 Jan 2020 16:52:57 GMT
CMD ["/bin/sh"]
# Fri, 20 Mar 2020 17:38:55 GMT
ARG VAULT_VERSION=1.3.4
# Fri, 20 Mar 2020 17:38:56 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN addgroup vault &&     adduser -S -G vault vault
# Fri, 20 Mar 2020 17:39:02 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Fri, 20 Mar 2020 17:39:03 GMT
# ARGS: VAULT_VERSION=1.3.4
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Fri, 20 Mar 2020 17:39:03 GMT
VOLUME [/vault/logs]
# Fri, 20 Mar 2020 17:39:03 GMT
VOLUME [/vault/file]
# Fri, 20 Mar 2020 17:39:03 GMT
EXPOSE 8200
# Fri, 20 Mar 2020 17:39:04 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Fri, 20 Mar 2020 17:39:04 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Fri, 20 Mar 2020 17:39:04 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:8ad089020f8a1fd366fb13feb183e2f4c7410e2232c54b40f6a54fd56029fdf3`  
		Last Modified: Thu, 23 Jan 2020 16:53:22 GMT  
		Size: 2.8 MB (2785861 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:195ddf817abf9b727a89d330e4c1749a26daa4f739a732b1f338eb5b3e6c2c47`  
		Last Modified: Fri, 20 Mar 2020 17:39:25 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9e7ed4e25c12c477182ca7df0f8dbe33a2a0d5e2d384b7b71ca2c042e7a8ce0`  
		Last Modified: Fri, 20 Mar 2020 17:39:33 GMT  
		Size: 47.3 MB (47322442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbbb751b023a72b97b2d81be1897efc8b90d04b9038332d55fd4eb5891700027`  
		Last Modified: Fri, 20 Mar 2020 17:39:24 GMT  
		Size: 155.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9279d72ca2647322e294804e55a4964b3941eac71139401ba6c3b1b4d9e72ce8`  
		Last Modified: Fri, 20 Mar 2020 17:39:24 GMT  
		Size: 1.8 KB (1824 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
