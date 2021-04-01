<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `vault`

-	[`vault:1.4.7`](#vault147)
-	[`vault:1.5.7`](#vault157)
-	[`vault:1.6.3`](#vault163)
-	[`vault:1.7.0`](#vault170)
-	[`vault:1.7.0-rc1`](#vault170-rc1)
-	[`vault:1.7.0-rc2`](#vault170-rc2)
-	[`vault:latest`](#vaultlatest)

## `vault:1.4.7`

```console
$ docker pull vault@sha256:5f83b42e92bc70e42f4183697efb20c4de6ab18e4b7e70c402ec031f7f2eb142
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.4.7` - linux; amd64

```console
$ docker pull vault@sha256:f52fc4392f247cb83afd90fb4ddc04cbaa77253ad5a1d03a03bc047e0effe493
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.1 MB (52081961 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:abdd06f0e819de997a424955ef9177a2db361e4ec2e8ee16d224eebe7e876817`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:25 GMT
ADD file:e944b37facf29902a466ebf545744be882c811e9501a8d2926393bd81a09b12a in / 
# Wed, 31 Mar 2021 20:10:25 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:32:08 GMT
ARG VAULT_VERSION=1.4.7
# Thu, 01 Apr 2021 17:32:09 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 17:32:14 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 17:32:16 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 17:32:16 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 17:32:16 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 17:32:16 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 17:32:16 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 17:32:17 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 17:32:17 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:bfdacc68c91b7e6d1aed01fb1262c6f752e85c932bd632e6bd62263818905ff9`  
		Last Modified: Wed, 31 Mar 2021 20:11:27 GMT  
		Size: 2.8 MB (2797176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a32b42ebd818e76620ae5d9b11506701b48afafdadc20fa4fef0b14b231bc675`  
		Last Modified: Thu, 01 Apr 2021 17:34:21 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b95b0160d074a3fed358e4984f6320a02d6ecfe28531c86088df0ae3f6a41aa6`  
		Last Modified: Thu, 01 Apr 2021 17:34:26 GMT  
		Size: 49.3 MB (49281491 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ab54dde68b0f0c36ddad6633a29287fee1a2d59d9b0952a23b1859bd6e2df79`  
		Last Modified: Thu, 01 Apr 2021 17:34:20 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78966ef53487d706f5eff8f172bbcd433d48ee06f80f301d8db3a8b9a41b0ee0`  
		Last Modified: Thu, 01 Apr 2021 17:34:19 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.7` - linux; arm variant v6

```console
$ docker pull vault@sha256:d0dca2f945d8e822b6a03243a6c4415616182dae7f7ff6c047800fb6d57c2f6e
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **48.7 MB (48719926 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:332eecd75d39566a3836c088ee1b7c0d91dc68b8d57ccabad4018b91e0773fca`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:28 GMT
ADD file:c67892974e87ac461e5f35f8cbbc4f25201ec62130f4e8691e52d79679fc10db in / 
# Wed, 31 Mar 2021 17:19:30 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:58:33 GMT
ARG VAULT_VERSION=1.4.7
# Thu, 01 Apr 2021 03:58:36 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 03:58:47 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 03:58:52 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 03:58:53 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 03:58:55 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 03:58:57 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 03:58:58 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 03:58:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 03:59:01 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:be6c23f3cb48f40fb3644ad115f4edc90f13074ffe485e8a6cdb64d36450000d`  
		Last Modified: Wed, 31 Mar 2021 17:20:28 GMT  
		Size: 2.6 MB (2574738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5d5f49a707d58744b3f2f9090c7b32ae943e59a356e14b1e34b3dc5ebcddc45`  
		Last Modified: Thu, 01 Apr 2021 04:01:14 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea79ab9087b53a729823f42ab9fb00712fb2c818e88ace527e3cc34eba2c41`  
		Last Modified: Thu, 01 Apr 2021 04:01:27 GMT  
		Size: 46.1 MB (46141890 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bacb85e2fcebdd7abec669bf90f60f7c743a67a54f8f7750154481a8dbbc85a7`  
		Last Modified: Thu, 01 Apr 2021 04:01:14 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f5348eb55f5cdf6d57790efcfa0a9ff2e43de7fa86c9c62561ea8db52e4c2781`  
		Last Modified: Thu, 01 Apr 2021 04:01:14 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.7` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:314ba67ffe528fd7e9306cfb3c1e382a56be4999e2fb70bb87f4337f2c3486f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **49.0 MB (48964610 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa699ae22e9b65a534abc51682ef9439e512a1738da8591579f5dc14bc823ed2`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:15 GMT
ADD file:f529d945837273af0ce4a7518436b3f6c988920c637e58b0c716d3c49c8007ad in / 
# Wed, 31 Mar 2021 17:22:16 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:21:51 GMT
ARG VAULT_VERSION=1.4.7
# Thu, 01 Apr 2021 16:21:53 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 16:22:00 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 16:22:03 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 16:22:04 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 16:22:05 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 16:22:06 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 16:22:07 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 16:22:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 16:22:10 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:9df31d96ae0cb1ae727e1c3d0ac9422da945cffd3f918f49a328911b2cbb0ba5`  
		Last Modified: Wed, 31 Mar 2021 17:23:09 GMT  
		Size: 2.7 MB (2720365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4fc362a50d3126eded1bba6e8afff39f85a6e7bba9bf238d8673ee929e785c84`  
		Last Modified: Thu, 01 Apr 2021 16:24:35 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:241af5b9d574c76339fde3b3274a6dfa368e96c4be66f5225c5beae45576ef35`  
		Last Modified: Thu, 01 Apr 2021 16:24:45 GMT  
		Size: 46.2 MB (46240949 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1e2d6aa1e5caf41834c777b37bd73298f75e3ec7738242f355ec40b6687edd2b`  
		Last Modified: Thu, 01 Apr 2021 16:24:35 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6dea14639788dab63974803c75d192dc2820c299f672c3bab6e22be72d919070`  
		Last Modified: Thu, 01 Apr 2021 16:24:35 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.4.7` - linux; 386

```console
$ docker pull vault@sha256:fd94a95b062e2263a6bb6a4acbbb4f068ef0b62334dfce2eb71a4fad60dac8e7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **50.2 MB (50214674 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:edaaf1726e365fbf040060e70a28136fb36703136ff9016c0cd09f2dc23dfa2a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:22 GMT
ADD file:7c227b0f23be0e208436424088c5275e9c1f6c62278ba35d6932e866af7cd534 in / 
# Wed, 31 Mar 2021 17:43:22 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 07:40:34 GMT
ARG VAULT_VERSION=1.4.7
# Thu, 01 Apr 2021 07:40:35 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 07:40:46 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 07:40:47 GMT
# ARGS: VAULT_VERSION=1.4.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 07:40:47 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 07:40:48 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 07:40:48 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 07:40:48 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 07:40:48 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 07:40:49 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:04a0b419ffe8e723a360cb667a2dace5907d4c994fb4da925108371a2936f954`  
		Last Modified: Wed, 31 Mar 2021 17:44:51 GMT  
		Size: 2.8 MB (2788886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d12935759d706f774b74906a761ee982e1b3c3c3c93f9494e97879acc4890ac5`  
		Last Modified: Thu, 01 Apr 2021 07:43:01 GMT  
		Size: 1.3 KB (1286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a9adc5f55a834e81d2a7e942d6eefcdacbf899e7a37c9e00cb79074eef121f0e`  
		Last Modified: Thu, 01 Apr 2021 07:43:07 GMT  
		Size: 47.4 MB (47422493 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc49f6a441aa3c2f0ae71a27ce2e2c82f332d26dead16f6a0ee8658b3991a9b9`  
		Last Modified: Thu, 01 Apr 2021 07:43:01 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e3d4915b3cded174f4bf62ac3895cd84bd76fea0f134c3df0e1806e5c95c673`  
		Last Modified: Thu, 01 Apr 2021 07:43:01 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.5.7`

```console
$ docker pull vault@sha256:4475bd10efb804c60135713f747dfe76817463cb9d996c77041453c8ef292258
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.5.7` - linux; amd64

```console
$ docker pull vault@sha256:a384f5c64cfd25e805511b07c83aa1bdd6263aed30b4b9738275f03af967e041
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **55.0 MB (55009996 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0e6922e274d28857552ecb9373665b3d70021a9f8abb0720725f7e1a54b6eec`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:25 GMT
ADD file:e944b37facf29902a466ebf545744be882c811e9501a8d2926393bd81a09b12a in / 
# Wed, 31 Mar 2021 20:10:25 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:31:55 GMT
ARG VAULT_VERSION=1.5.7
# Thu, 01 Apr 2021 17:31:56 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 17:32:02 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 17:32:04 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 17:32:04 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 17:32:04 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 17:32:04 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 17:32:04 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 17:32:05 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 17:32:05 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:bfdacc68c91b7e6d1aed01fb1262c6f752e85c932bd632e6bd62263818905ff9`  
		Last Modified: Wed, 31 Mar 2021 20:11:27 GMT  
		Size: 2.8 MB (2797176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4511bdb3b11c02e1b03aaa0f71b32f05403c0d87db709f7bab0216e18d2a5d77`  
		Last Modified: Thu, 01 Apr 2021 17:33:58 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0d4d771fd86121b4bf584ad43d90f06718735a9e23bfdb29c48123b7819113f`  
		Last Modified: Thu, 01 Apr 2021 17:34:05 GMT  
		Size: 52.2 MB (52209526 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ad7e9386d924f12f8a7ffe1a21711ea32aa7fbf7681cf2ef6b0b53851024ea9`  
		Last Modified: Thu, 01 Apr 2021 17:33:58 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc0e34e699e48358659ec8dd61bd72f477923fe14a62318136c6e8dc41070440`  
		Last Modified: Thu, 01 Apr 2021 17:33:58 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.7` - linux; arm variant v6

```console
$ docker pull vault@sha256:3357d3045a27aa29c392cd93bae177ad9391598ee4fd35c4e62cd24cc7847401
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.6 MB (51563662 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:febf1562db612f245583630216a74b0e1ebdb85a97310e8b7f82f404ee5b8e57`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:19:28 GMT
ADD file:c67892974e87ac461e5f35f8cbbc4f25201ec62130f4e8691e52d79679fc10db in / 
# Wed, 31 Mar 2021 17:19:30 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:57:59 GMT
ARG VAULT_VERSION=1.5.7
# Thu, 01 Apr 2021 03:58:03 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 03:58:14 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 03:58:18 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 03:58:19 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 03:58:21 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 03:58:21 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 03:58:22 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 03:58:24 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 03:58:25 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:be6c23f3cb48f40fb3644ad115f4edc90f13074ffe485e8a6cdb64d36450000d`  
		Last Modified: Wed, 31 Mar 2021 17:20:28 GMT  
		Size: 2.6 MB (2574738 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f8c983a5d00827bd572e20fc04f3b39fc56a3d650e35bf1679a95b85209d50f`  
		Last Modified: Thu, 01 Apr 2021 04:00:51 GMT  
		Size: 1.3 KB (1289 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cbfa587963d2764da1967eeba7dce68b51ffa2523c024d632ca6e7f93f658129`  
		Last Modified: Thu, 01 Apr 2021 04:01:04 GMT  
		Size: 49.0 MB (48985628 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49da638d8131344e1b62846c51c54389349d6cfa71a20fb24f3e818975032e17`  
		Last Modified: Thu, 01 Apr 2021 04:00:51 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2d162537167491a21b4cee6e7262250273c6088e550411f6915420050dc37006`  
		Last Modified: Thu, 01 Apr 2021 04:00:51 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.7` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:feebe282b3fae77172bb2b4c83f9e7eeeaee4b027efcadf20cde8dd9a402d824
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **51.9 MB (51918019 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f517a07066fcfc11cd67c0537a36e78612819bada285fee6577257e57a77c3a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:22:15 GMT
ADD file:f529d945837273af0ce4a7518436b3f6c988920c637e58b0c716d3c49c8007ad in / 
# Wed, 31 Mar 2021 17:22:16 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:21:24 GMT
ARG VAULT_VERSION=1.5.7
# Thu, 01 Apr 2021 16:21:26 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 16:21:34 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 16:21:37 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 16:21:38 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 16:21:39 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 16:21:40 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 16:21:42 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 16:21:43 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 16:21:44 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:9df31d96ae0cb1ae727e1c3d0ac9422da945cffd3f918f49a328911b2cbb0ba5`  
		Last Modified: Wed, 31 Mar 2021 17:23:09 GMT  
		Size: 2.7 MB (2720365 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00dadb0c70a4c7c2232fbd3a7b719978636e907afa8cf5dc7b92f223861f8197`  
		Last Modified: Thu, 01 Apr 2021 16:24:15 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e1a42756bbe1b1be68c57c00a859d73813bf3b48d1fdacc5ef40410db2e6c301`  
		Last Modified: Thu, 01 Apr 2021 16:24:29 GMT  
		Size: 49.2 MB (49194357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65601366d0fe0bceb842d0c0da41112e7338fc0e22d5a3515e8dd8b09e21518c`  
		Last Modified: Thu, 01 Apr 2021 16:24:12 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cf2f95661862dffc826891296c1f3c3f92d3b15f0ca422545ef71cf853eaebe9`  
		Last Modified: Thu, 01 Apr 2021 16:24:12 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.5.7` - linux; 386

```console
$ docker pull vault@sha256:8d53fdcfb6eb252827d4f8c2410b7ab39ddc84ac75d92997418edabb3158e7ab
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **53.1 MB (53087413 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3fc0466cda58f7b40445e9c0dfbdf883b7cfaecf277ce6f141ea95c5d479a5fe`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:22 GMT
ADD file:7c227b0f23be0e208436424088c5275e9c1f6c62278ba35d6932e866af7cd534 in / 
# Wed, 31 Mar 2021 17:43:22 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 07:40:18 GMT
ARG VAULT_VERSION=1.5.7
# Thu, 01 Apr 2021 07:40:19 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 07:40:26 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 07:40:27 GMT
# ARGS: VAULT_VERSION=1.5.7
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 07:40:27 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 07:40:28 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 07:40:28 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 07:40:28 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 07:40:28 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 07:40:29 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:04a0b419ffe8e723a360cb667a2dace5907d4c994fb4da925108371a2936f954`  
		Last Modified: Wed, 31 Mar 2021 17:44:51 GMT  
		Size: 2.8 MB (2788886 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1d4c93180af1ac026f74867f66f738819c3a6c5f61ce7c1a055d025fe25326fd`  
		Last Modified: Thu, 01 Apr 2021 07:42:42 GMT  
		Size: 1.3 KB (1288 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ea8ba055ad0de265a31174c8fb41a36721f210f7021d624f174a48ba13c0ccd`  
		Last Modified: Thu, 01 Apr 2021 07:42:51 GMT  
		Size: 50.3 MB (50295233 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:296db6c0defdd53542aeb869240130df1474e3e19a6659675aabcea35d6b0159`  
		Last Modified: Thu, 01 Apr 2021 07:42:42 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9552c0192dae283787dea14ffad97c75386c9c308b42100c6595c0509dc0f5ee`  
		Last Modified: Thu, 01 Apr 2021 07:42:43 GMT  
		Size: 1.8 KB (1818 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.6.3`

```console
$ docker pull vault@sha256:5b06041ee0c2c5f1039afe53d5ee55af5b1c30c1ff17aab8c979e972237adb10
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.6.3` - linux; amd64

```console
$ docker pull vault@sha256:b2af2dbdc5da480bf4080c6ce4a6480dde96cd97a363f0ddfb8b50c385fe7ccb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **69.0 MB (68983158 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:46bde53c0ee0a4070e090105678ff09fe21ef235f43a85f34cb3709cb4b1a217`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:31:42 GMT
ARG VAULT_VERSION=1.6.3
# Thu, 01 Apr 2021 17:31:43 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 17:31:49 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 17:31:51 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 17:31:51 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 17:31:51 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 17:31:51 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 17:31:51 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 17:31:52 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 17:31:52 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f3af05648f31c8c2f0208bede8af2461cb74da99bd21dd8b75f38fc33c8a34b`  
		Last Modified: Thu, 01 Apr 2021 17:33:35 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3b8ee63da96697cf9742be50bc6c46cfdb8f0a2599fdd0f50660c7bbd24ccbc`  
		Last Modified: Thu, 01 Apr 2021 17:33:45 GMT  
		Size: 66.2 MB (66167944 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69d8d257f696a3b3f0524fe3e522f51a9199c55e4e8475a94f6e7a29cdedf05e`  
		Last Modified: Thu, 01 Apr 2021 17:33:36 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:667f3060e41e3f39c8a96a35b38f0ba1cd50428a4e7e5291b819398c5ff0a62d`  
		Last Modified: Thu, 01 Apr 2021 17:33:38 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.3` - linux; arm variant v6

```console
$ docker pull vault@sha256:af3df371e4c0af651fa91ed7fa02eda3d25caa5f02b7a545bee9769e4467fa94
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.7 MB (63718984 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4f3a600bd0006785302e582f039df932398490653cff3ccc7e525751a901e96f`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:57:28 GMT
ARG VAULT_VERSION=1.6.3
# Thu, 01 Apr 2021 03:57:30 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 03:57:42 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 03:57:45 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 03:57:46 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 03:57:47 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 03:57:48 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 03:57:49 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 03:57:49 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 03:57:50 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39ce309e6e5a01b40af1594950ece8755a1bfe5379c7691aed095109f568c05b`  
		Last Modified: Thu, 01 Apr 2021 04:00:29 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9dc750f866fd134ec1f96948dbd2e62a9cfd08868d3b162e0034ff22e3463578`  
		Last Modified: Thu, 01 Apr 2021 04:00:44 GMT  
		Size: 61.1 MB (61093605 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97926d0b63a116ed6da0e06032e50ff30a5c5d794fa401841a7dfb1e8101e95a`  
		Last Modified: Thu, 01 Apr 2021 04:00:29 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:01c300997714121a041f195730b3bdcefccd443081666432fe426b57feb9376a`  
		Last Modified: Thu, 01 Apr 2021 04:00:29 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.3` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:f96fdc3812a2dbb974e667aab06a11ee9c1996db6212c41537f53b8aab040111
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **65.0 MB (65016303 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0657c4de016c6846745e808c2050470208abaacb0f5df4261cbc02712fb1f76e`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:20:56 GMT
ARG VAULT_VERSION=1.6.3
# Thu, 01 Apr 2021 16:20:59 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 16:21:08 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 16:21:11 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 16:21:12 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 16:21:13 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 16:21:14 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 16:21:15 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 16:21:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 16:21:17 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d99e98fb7e11512ea009aec5c95e39caceb3c4a3138932bb7f851c570975a9a5`  
		Last Modified: Thu, 01 Apr 2021 16:23:46 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3aff431808a8ad8bed1f967d6e58d97d91f96df02eb7ec16307ac250065e2f4a`  
		Last Modified: Thu, 01 Apr 2021 16:24:00 GMT  
		Size: 62.3 MB (62301117 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:728d08c934fc1fada6704e9660661e48e9f5aaabb8712edd0237c93fd0a06827`  
		Last Modified: Thu, 01 Apr 2021 16:23:47 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb3bebac8d1d926f0c8fafe4b39c637b98f76f5962284055bc1898bac9df34a`  
		Last Modified: Thu, 01 Apr 2021 16:23:46 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.6.3` - linux; 386

```console
$ docker pull vault@sha256:264ad1c2dc56cee7d0084792d154b6d0ebeba6a3803e889a92da3e8657b67d78
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **67.0 MB (67033806 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f7b003192a1cc10541ddc869e8ffe0939d4ceed0c257cad42caca94852bedbcd`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 07:39:51 GMT
ARG VAULT_VERSION=1.6.3
# Thu, 01 Apr 2021 07:39:51 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 07:40:09 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 07:40:10 GMT
# ARGS: VAULT_VERSION=1.6.3
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 07:40:11 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 07:40:11 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 07:40:11 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 07:40:11 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 07:40:12 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 07:40:12 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bd19dd98dc640a3767602128f49255ee769d83548842d11ad6e3ef1740b2619`  
		Last Modified: Thu, 01 Apr 2021 07:42:18 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:805151cbb986e3fcd3f9d86bd93e662de8bf352ab4834e0b3f40b14d09798bbd`  
		Last Modified: Thu, 01 Apr 2021 07:42:33 GMT  
		Size: 64.2 MB (64211740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:51c20b08ef78c8b4dda1c38c8fbe81144c2e60fb8e271ba14415e7b9cdefe6e4`  
		Last Modified: Thu, 01 Apr 2021 07:42:18 GMT  
		Size: 187.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8902e15ecbb84df8e81b22cb54101ab6a1ca6a5def92f186ba2cde9857e6d42`  
		Last Modified: Thu, 01 Apr 2021 07:42:18 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.7.0`

```console
$ docker pull vault@sha256:635cf1c3f9b10fe03aad375f94cc61f63d74a189662165285a8bf1c189ea04b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.7.0` - linux; amd64

```console
$ docker pull vault@sha256:b374bf9a8d703434241a265ffd5a158849f074b53136631073b2adfe852d8568
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72706980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88d9c1800228240e26c6fcfe2b802377372bd3137477e956d04136bd09f1c850`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:30:57 GMT
ARG VAULT_VERSION=1.7.0
# Thu, 01 Apr 2021 17:30:58 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 17:31:05 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 17:31:07 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 17:31:07 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 17:31:07 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 17:31:07 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 17:31:08 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 17:31:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 17:31:08 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd267b6ea9bab98e28e9c82a7d40d2c96968afffb2dfd5429e4f7c757fe48ce`  
		Last Modified: Thu, 01 Apr 2021 17:32:35 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521e6c56e0e818f333cfd641cb801c58904b4705c539ba31bb4ad03d23ddf1c9`  
		Last Modified: Thu, 01 Apr 2021 17:32:41 GMT  
		Size: 69.9 MB (69891766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80adec01e0450732ba24cc8b51581339e5543f9229a3066971043dc04e0d606`  
		Last Modified: Thu, 01 Apr 2021 17:32:31 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecae57e5555d3cca6a1ac593e1f642e3065fdcfb64364dac536a72d510f2dd6`  
		Last Modified: Thu, 01 Apr 2021 17:32:31 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.0` - linux; arm variant v6

```console
$ docker pull vault@sha256:767919f77e45c4294de6e32d3b893b5036c762e51d560b76330932192e404d2f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66726620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc8bde904bf2e29386a8fb240f6b1fb95f45ebf9d38f7fe2077517b1b514eb4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:55:36 GMT
ARG VAULT_VERSION=1.7.0
# Thu, 01 Apr 2021 03:55:38 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 03:55:51 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 03:55:54 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 03:55:55 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 03:55:56 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 03:55:57 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 03:55:58 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 03:55:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 03:55:59 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad73fe886cac5dcb33a379031cfe005dda18d2607759d02d567e1a7f3f92dbdc`  
		Last Modified: Thu, 01 Apr 2021 03:59:20 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5ffa7fbdf0fe366fdafb6a2123b019f1febe00b3c8ce5ab4c74d95b9b1512d`  
		Last Modified: Thu, 01 Apr 2021 03:59:36 GMT  
		Size: 64.1 MB (64101238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0d98dbcea4800176a5738fab3df0551316a16e5268fb5cc21cdf4b308ab390`  
		Last Modified: Thu, 01 Apr 2021 03:59:20 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9187438e2855de2e5af03cd0105dd1eb20593f9ad6f0b5f166eb83324d20402`  
		Last Modified: Thu, 01 Apr 2021 03:59:20 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.0` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:077bfdb5884893f1ef36cd00c2a17fe536424a1987e03f81aaadd306a4449172
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68535710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1778579c7a3692819b8c4e60f6498730d670cb31183f446873944ae3a84af8e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:19:26 GMT
ARG VAULT_VERSION=1.7.0
# Thu, 01 Apr 2021 16:19:28 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 16:19:37 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 16:19:41 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 16:19:41 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 16:19:42 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 16:19:43 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 16:19:44 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 16:19:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 16:19:46 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a79508f0f3b568f24de2552c1f66ddd401aa0413c3dd7a4efc2f75a254a47e5`  
		Last Modified: Thu, 01 Apr 2021 16:22:32 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268e70bba78db02cf6d0d5e808b06ca5de2b84b044e6e05361c9b3c3d2f68dfd`  
		Last Modified: Thu, 01 Apr 2021 16:22:47 GMT  
		Size: 65.8 MB (65820525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365b501ce314391fe9031e1189b1b44303176b3a9831682604ecb617e85e67af`  
		Last Modified: Thu, 01 Apr 2021 16:22:32 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648ce37fd7d6009b59b5114f8ffebf912386c534a6b04a3edb126781a4123faa`  
		Last Modified: Thu, 01 Apr 2021 16:22:32 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.0` - linux; 386

```console
$ docker pull vault@sha256:d36e98f13ac378cbfe847d7b589b64f2bada4f3ff90bdb8104989158840c981d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70570703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84c26749e2878226c02eeba1c262288c19c01cc6d0684b9bab0b810254544e25`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 07:38:55 GMT
ARG VAULT_VERSION=1.7.0
# Thu, 01 Apr 2021 07:38:56 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 07:39:08 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 07:39:09 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 07:39:09 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 07:39:10 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 07:39:10 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 07:39:10 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 07:39:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 07:39:11 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253b6fe11e847937b3bb907714a7ba2d39bfe7574e23a0b57a5492261959a9ca`  
		Last Modified: Thu, 01 Apr 2021 07:41:16 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ee58c78adb286aa02cf737f3ef4e76eaaa4501219874cc1b1edd91955ab2e8`  
		Last Modified: Thu, 01 Apr 2021 07:41:29 GMT  
		Size: 67.7 MB (67748638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc29516badcc93e7963cd6ac28767a2e3d4cc53aa6da2393e8e786479ef11c41`  
		Last Modified: Thu, 01 Apr 2021 07:41:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e4c24c4948e932b7b5761fe9af854282834a76e1e7d7f24267473911695c8e`  
		Last Modified: Thu, 01 Apr 2021 07:41:16 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.7.0-rc1`

```console
$ docker pull vault@sha256:d6a743ae3cac9b0b0aa27ed53c019932b3c8ed826c3342aa6d7fbaaa27666a90
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.7.0-rc1` - linux; amd64

```console
$ docker pull vault@sha256:5e7a1c5639469b46f018b8a58db6b71723f91e38ac39453b2f780e6217f30acb
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72670858 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3324468db92c90e509490f2c7b66353fd00f037aed33314ca62f0337c6b24914`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:31:24 GMT
ARG VAULT_VERSION=1.7.0-rc1
# Thu, 01 Apr 2021 17:31:25 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 17:31:36 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 17:31:37 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 17:31:38 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 17:31:38 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 17:31:38 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 17:31:38 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 17:31:38 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 17:31:39 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3977c769ed5dbb08783e15a597716b34a3e268788d6aa1e9a14454910207abb0`  
		Last Modified: Thu, 01 Apr 2021 17:33:19 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd896bf3500bfff124fc5a6f6243b40826a5141ab68d232272e49fc840081de3`  
		Last Modified: Thu, 01 Apr 2021 17:33:27 GMT  
		Size: 69.9 MB (69855648 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cac2a63f6784c6c8e18465ee29cdc55854c65a5d07635bb4cdb4009274de94a`  
		Last Modified: Thu, 01 Apr 2021 17:33:18 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebaf5d7e7500d5461c2b91d266e346852edbdc837354f7c4d2c69189ac352eef`  
		Last Modified: Thu, 01 Apr 2021 17:33:19 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.0-rc1` - linux; arm variant v6

```console
$ docker pull vault@sha256:5f2104257d57fa6d0cfda5db2be3a8991d3e88009ef1e01f7029bdda9b1a6dc7
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66701345 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:bd2babc4a35ac6d29f28f5f7de7af65a8c80442569cc94af14127b36f1d7c8cf`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:56:45 GMT
ARG VAULT_VERSION=1.7.0-rc1
# Thu, 01 Apr 2021 03:56:48 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 03:57:02 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 03:57:10 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 03:57:11 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 03:57:12 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 03:57:13 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 03:57:14 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 03:57:16 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 03:57:17 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba5ba71ddedad5e323c1fcf258f7f81d053635d689060ade0c9a8cac0ad970de`  
		Last Modified: Thu, 01 Apr 2021 04:00:08 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19f55bab30045ce5ff32810fbd51e7bc6fc6564daa660437e4570d0abd26e10a`  
		Last Modified: Thu, 01 Apr 2021 04:00:24 GMT  
		Size: 64.1 MB (64075962 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c57c74fdb785c3b36ec26f0eb2a7a9012f348fdca66fdc15380298df89798d5e`  
		Last Modified: Thu, 01 Apr 2021 04:00:07 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5310f0f572a9d76a9f33bfdbc38e7262b3ea318ee0f5e9ff8d5e94929ac592c5`  
		Last Modified: Thu, 01 Apr 2021 04:00:07 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.0-rc1` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:c4fe93ae7584b2f9640279e193d44fc4d17e4b177ccfeef7e1f13c79a3507b48
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68500292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1585283faab2410e0584f2d027a96ee9158677262c71c86a36a095316a9d588d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:20:25 GMT
ARG VAULT_VERSION=1.7.0-rc1
# Thu, 01 Apr 2021 16:20:27 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 16:20:38 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 16:20:41 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 16:20:42 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 16:20:43 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 16:20:43 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 16:20:44 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 16:20:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 16:20:46 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5157b4652970a2aabcbfd59b177507b07ed0e3bf4acf937dd1979aada36b1678`  
		Last Modified: Thu, 01 Apr 2021 16:23:19 GMT  
		Size: 1.3 KB (1259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ffca5a23916c0f28a2a43acabe5440eca87590451369d62bebee54f6841cb39`  
		Last Modified: Thu, 01 Apr 2021 16:23:40 GMT  
		Size: 65.8 MB (65785104 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9aad453ae6f0cb91db19629a342b9f6f5be1b6a958386ca955b4f145917dc5fe`  
		Last Modified: Thu, 01 Apr 2021 16:23:21 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e39bef7c305aa78355f52390afa87c87f60773b3dae161fd8705b8ce50de413c`  
		Last Modified: Thu, 01 Apr 2021 16:23:21 GMT  
		Size: 1.8 KB (1823 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.0-rc1` - linux; 386

```console
$ docker pull vault@sha256:81a15f9c8805e7842995786b8244bd1bc05ef58aa4d438f65b17418ac188a393
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70535844 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9ab538c608b36b5fe509039ff7578630cd153d3e82aa30c56e32418ae83f9e9d`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 07:39:34 GMT
ARG VAULT_VERSION=1.7.0-rc1
# Thu, 01 Apr 2021 07:39:35 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 07:39:43 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 07:39:44 GMT
# ARGS: VAULT_VERSION=1.7.0-rc1
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 07:39:45 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 07:39:45 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 07:39:45 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 07:39:45 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 07:39:46 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 07:39:46 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:590eaae62029bf0be7673568af39ccfcaa2bd1e816d4112c516c841cd285fcd8`  
		Last Modified: Thu, 01 Apr 2021 07:42:00 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:68ff76ea2cca657b626fdbd0e292c098cd6cef2ecb25dd00f523dd452c4fdb10`  
		Last Modified: Thu, 01 Apr 2021 07:42:10 GMT  
		Size: 67.7 MB (67713778 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a703ee07424215cd277d1d6d47504f925b4ab6a33a1a8c0d6db0db966ca8ac6d`  
		Last Modified: Thu, 01 Apr 2021 07:42:01 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5696e88fe90abfaad846797c87afbb0587c321b5d5cffa1aa1989e2152e84d0`  
		Last Modified: Thu, 01 Apr 2021 07:42:00 GMT  
		Size: 1.8 KB (1819 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:1.7.0-rc2`

```console
$ docker pull vault@sha256:cb2154a91297964b77086e716c1763617123dc8cd9655b74f9fdffa09fd0e844
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:1.7.0-rc2` - linux; amd64

```console
$ docker pull vault@sha256:a11019640cd665bd4952ffff33f1b292c7150ed92600ff0e09720dd6e68612fe
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72667657 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d66ea79f14f3c24271306ed4bffa10ab600787944aa1d4248b3438123ee7e294`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:31:11 GMT
ARG VAULT_VERSION=1.7.0-rc2
# Thu, 01 Apr 2021 17:31:12 GMT
# ARGS: VAULT_VERSION=1.7.0-rc2
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 17:31:19 GMT
# ARGS: VAULT_VERSION=1.7.0-rc2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 17:31:20 GMT
# ARGS: VAULT_VERSION=1.7.0-rc2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 17:31:20 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 17:31:20 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 17:31:21 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 17:31:21 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 17:31:21 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 17:31:21 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fc3a1c636e9c016d4c615c953dcc1a6d8d199f70dff5a786f5fd5f413acb5c30`  
		Last Modified: Thu, 01 Apr 2021 17:32:57 GMT  
		Size: 1.3 KB (1256 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b9d40cbdee16e3bc781c3cbb342f037d4a3691da2dbb9d7a7d51f229a7410a3d`  
		Last Modified: Thu, 01 Apr 2021 17:33:09 GMT  
		Size: 69.9 MB (69852446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9953512c38e5a1e3f1474f34477e41a0a4d1da19ea72671693b9b18557ded169`  
		Last Modified: Thu, 01 Apr 2021 17:32:57 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5197f526d0769ffb41ba51796254172f7282b76ace7b374043df6361a214dfde`  
		Last Modified: Thu, 01 Apr 2021 17:32:57 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.0-rc2` - linux; arm variant v6

```console
$ docker pull vault@sha256:dd84b8beb1d5d365ac3fcf37eb36a5566281d0e7175325c7ad4ee705c293d2f3
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66702771 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b8f445612edbef36da3cbe796108934b166458052bf4af3d37c956e5b2554434`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:56:08 GMT
ARG VAULT_VERSION=1.7.0-rc2
# Thu, 01 Apr 2021 03:56:11 GMT
# ARGS: VAULT_VERSION=1.7.0-rc2
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 03:56:25 GMT
# ARGS: VAULT_VERSION=1.7.0-rc2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 03:56:29 GMT
# ARGS: VAULT_VERSION=1.7.0-rc2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 03:56:30 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 03:56:31 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 03:56:32 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 03:56:34 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 03:56:35 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 03:56:36 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:50f930327c92277e0956645dc2f700c5bcb45bd3df1dc7ca6fa710e4c954b7c8`  
		Last Modified: Thu, 01 Apr 2021 03:59:44 GMT  
		Size: 1.3 KB (1261 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f77723b385f3c34e858e442810c83498a93b11396e952d2c1e812034979eb1e`  
		Last Modified: Thu, 01 Apr 2021 04:00:00 GMT  
		Size: 64.1 MB (64077386 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c39c772f5c36d7308d31a9835fbdc4cdc1d80225c48ebe3db1d3624f5155896`  
		Last Modified: Thu, 01 Apr 2021 03:59:44 GMT  
		Size: 186.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c1ab94140bc7099cf76311c54014077beb69bd9e1b64d28f231eb76f9c30a4f8`  
		Last Modified: Thu, 01 Apr 2021 03:59:44 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.0-rc2` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:6b54883870c88aa1e27b6584a822ccb1b69c12a5295c53abbfeff28ff43234fc
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68525649 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3083656cea832a018d87a62ea8ca2959949add71a752eb4dc73c2c875a3ca0ad`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:19:54 GMT
ARG VAULT_VERSION=1.7.0-rc2
# Thu, 01 Apr 2021 16:19:56 GMT
# ARGS: VAULT_VERSION=1.7.0-rc2
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 16:20:06 GMT
# ARGS: VAULT_VERSION=1.7.0-rc2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 16:20:09 GMT
# ARGS: VAULT_VERSION=1.7.0-rc2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 16:20:10 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 16:20:11 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 16:20:12 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 16:20:13 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 16:20:14 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 16:20:15 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1b8c37832e2d24b66cc163875c85c3135db34ec764cd429334a9c17c1e9cf057`  
		Last Modified: Thu, 01 Apr 2021 16:22:58 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ef298bfb7b70319b313e366e36a306d189b8295aebe14ef43e08f7d039cc3ea6`  
		Last Modified: Thu, 01 Apr 2021 16:23:12 GMT  
		Size: 65.8 MB (65810462 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b53ba185fd193cee56ce8dc27aeae0ef80da77749ea89cfd63f41c5cdd99fc92`  
		Last Modified: Thu, 01 Apr 2021 16:22:58 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521d88c82dd678288f8653c316238b3ffc725403e5a4f4b502f85cb1bdc16aec`  
		Last Modified: Thu, 01 Apr 2021 16:22:58 GMT  
		Size: 1.8 KB (1822 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:1.7.0-rc2` - linux; 386

```console
$ docker pull vault@sha256:437cd8adf9f2d358600e56ee007e6a573848784d3e82560bf1e1d034ef16cef6
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.5 MB (70540267 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:37877c15431950f167453c2017945c1c86c7d5a6f2ace2db9c46700547d9a261`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 07:39:17 GMT
ARG VAULT_VERSION=1.7.0-rc2
# Thu, 01 Apr 2021 07:39:18 GMT
# ARGS: VAULT_VERSION=1.7.0-rc2
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 07:39:26 GMT
# ARGS: VAULT_VERSION=1.7.0-rc2
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 07:39:28 GMT
# ARGS: VAULT_VERSION=1.7.0-rc2
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 07:39:28 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 07:39:28 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 07:39:28 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 07:39:29 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 07:39:29 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 07:39:29 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fbbf718bb3dabb9e2dc5fcce8ab3d30bd37469858b9983d02221ed8147d3398`  
		Last Modified: Thu, 01 Apr 2021 07:41:43 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d23dffce4eec8032ff13f7e4455b865dfee11863441720e87194f375f9133ee7`  
		Last Modified: Thu, 01 Apr 2021 07:41:50 GMT  
		Size: 67.7 MB (67718199 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a4b82687d428025e6098a9059e35fe51f6cfcc879dba5e5c564bb0ca30eb99d`  
		Last Modified: Thu, 01 Apr 2021 07:41:43 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b3780390f30b878bc253ddec7f011e7015de79d32a0db39398d89aee6db2e838`  
		Last Modified: Thu, 01 Apr 2021 07:41:40 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `vault:latest`

```console
$ docker pull vault@sha256:635cf1c3f9b10fe03aad375f94cc61f63d74a189662165285a8bf1c189ea04b8
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386

### `vault:latest` - linux; amd64

```console
$ docker pull vault@sha256:b374bf9a8d703434241a265ffd5a158849f074b53136631073b2adfe852d8568
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **72.7 MB (72706980 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:88d9c1800228240e26c6fcfe2b802377372bd3137477e956d04136bd09f1c850`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 20:10:06 GMT
ADD file:7119167b56ff1228b2fb639c768955ce9db7a999cd947179240b216dfa5ccbb9 in / 
# Wed, 31 Mar 2021 20:10:06 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 17:30:57 GMT
ARG VAULT_VERSION=1.7.0
# Thu, 01 Apr 2021 17:30:58 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 17:31:05 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 17:31:07 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 17:31:07 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 17:31:07 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 17:31:07 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 17:31:08 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 17:31:08 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 17:31:08 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:ca3cd42a7c9525f6ce3d64c1a70982613a8235f0cc057ec9244052921853ef15`  
		Last Modified: Wed, 31 Mar 2021 20:10:46 GMT  
		Size: 2.8 MB (2811947 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bd267b6ea9bab98e28e9c82a7d40d2c96968afffb2dfd5429e4f7c757fe48ce`  
		Last Modified: Thu, 01 Apr 2021 17:32:35 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:521e6c56e0e818f333cfd641cb801c58904b4705c539ba31bb4ad03d23ddf1c9`  
		Last Modified: Thu, 01 Apr 2021 17:32:41 GMT  
		Size: 69.9 MB (69891766 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e80adec01e0450732ba24cc8b51581339e5543f9229a3066971043dc04e0d606`  
		Last Modified: Thu, 01 Apr 2021 17:32:31 GMT  
		Size: 190.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9ecae57e5555d3cca6a1ac593e1f642e3065fdcfb64364dac536a72d510f2dd6`  
		Last Modified: Thu, 01 Apr 2021 17:32:31 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm variant v6

```console
$ docker pull vault@sha256:767919f77e45c4294de6e32d3b893b5036c762e51d560b76330932192e404d2f
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **66.7 MB (66726620 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:dc8bde904bf2e29386a8fb240f6b1fb95f45ebf9d38f7fe2077517b1b514eb4a`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:18:49 GMT
ADD file:988879d74f643b89539e5a0b6d74221621f19f4f87f722614addadc46ce47200 in / 
# Wed, 31 Mar 2021 17:18:50 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 03:55:36 GMT
ARG VAULT_VERSION=1.7.0
# Thu, 01 Apr 2021 03:55:38 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 03:55:51 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 03:55:54 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 03:55:55 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 03:55:56 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 03:55:57 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 03:55:58 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 03:55:59 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 03:55:59 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:bb87125c6ee1ce30c6b33d2c96a9fbe46da4a290f7cb1dd73fd62d4e06503699`  
		Last Modified: Wed, 31 Mar 2021 17:19:55 GMT  
		Size: 2.6 MB (2622116 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad73fe886cac5dcb33a379031cfe005dda18d2607759d02d567e1a7f3f92dbdc`  
		Last Modified: Thu, 01 Apr 2021 03:59:20 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e5ffa7fbdf0fe366fdafb6a2123b019f1febe00b3c8ce5ab4c74d95b9b1512d`  
		Last Modified: Thu, 01 Apr 2021 03:59:36 GMT  
		Size: 64.1 MB (64101238 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7f0d98dbcea4800176a5738fab3df0551316a16e5268fb5cc21cdf4b308ab390`  
		Last Modified: Thu, 01 Apr 2021 03:59:20 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9187438e2855de2e5af03cd0105dd1eb20593f9ad6f0b5f166eb83324d20402`  
		Last Modified: Thu, 01 Apr 2021 03:59:20 GMT  
		Size: 1.8 KB (1821 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; arm64 variant v8

```console
$ docker pull vault@sha256:077bfdb5884893f1ef36cd00c2a17fe536424a1987e03f81aaadd306a4449172
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **68.5 MB (68535710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1778579c7a3692819b8c4e60f6498730d670cb31183f446873944ae3a84af8e3`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:21:21 GMT
ADD file:3b16ffee2b26d8af5db152fcc582aaccd9e1ec9e3343874e9969a205550fe07d in / 
# Wed, 31 Mar 2021 17:21:23 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 16:19:26 GMT
ARG VAULT_VERSION=1.7.0
# Thu, 01 Apr 2021 16:19:28 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 16:19:37 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 16:19:41 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 16:19:41 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 16:19:42 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 16:19:43 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 16:19:44 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 16:19:45 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 16:19:46 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:912815139b61c8926da31f7701f0a924e7964e3713052bf1a53193a4562157f6`  
		Last Modified: Wed, 31 Mar 2021 17:22:41 GMT  
		Size: 2.7 MB (2711920 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4a79508f0f3b568f24de2552c1f66ddd401aa0413c3dd7a4efc2f75a254a47e5`  
		Last Modified: Thu, 01 Apr 2021 16:22:32 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:268e70bba78db02cf6d0d5e808b06ca5de2b84b044e6e05361c9b3c3d2f68dfd`  
		Last Modified: Thu, 01 Apr 2021 16:22:47 GMT  
		Size: 65.8 MB (65820525 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:365b501ce314391fe9031e1189b1b44303176b3a9831682604ecb617e85e67af`  
		Last Modified: Thu, 01 Apr 2021 16:22:32 GMT  
		Size: 188.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:648ce37fd7d6009b59b5114f8ffebf912386c534a6b04a3edb126781a4123faa`  
		Last Modified: Thu, 01 Apr 2021 16:22:32 GMT  
		Size: 1.8 KB (1820 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `vault:latest` - linux; 386

```console
$ docker pull vault@sha256:d36e98f13ac378cbfe847d7b589b64f2bada4f3ff90bdb8104989158840c981d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **70.6 MB (70570703 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:84c26749e2878226c02eeba1c262288c19c01cc6d0684b9bab0b810254544e25`
-	Entrypoint: `["docker-entrypoint.sh"]`
-	Default Command: `["server","-dev"]`

```dockerfile
# Wed, 31 Mar 2021 17:43:00 GMT
ADD file:245767f958e2b5e6fad41d45d3361849e7c6b2255303e3c785f0f2c86019553a in / 
# Wed, 31 Mar 2021 17:43:00 GMT
CMD ["/bin/sh"]
# Thu, 01 Apr 2021 07:38:55 GMT
ARG VAULT_VERSION=1.7.0
# Thu, 01 Apr 2021 07:38:56 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN addgroup vault &&     adduser -S -G vault vault
# Thu, 01 Apr 2021 07:39:08 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN set -eux;     apk add --no-cache ca-certificates gnupg openssl libcap su-exec dumb-init tzdata &&     apkArch="$(apk --print-arch)";     case "$apkArch" in         armhf) ARCH='arm' ;;         aarch64) ARCH='arm64' ;;         x86_64) ARCH='amd64' ;;         x86) ARCH='386' ;;         *) echo >&2 "error: unsupported architecture: $apkArch"; exit 1 ;;     esac &&     VAULT_GPGKEY=91A6E7F85D05C65630BEF18951852D87348FFC4C;     found='';     for server in         hkp://p80.pool.sks-keyservers.net:80         hkp://keyserver.ubuntu.com:80         hkp://pgp.mit.edu:80     ; do         echo "Fetching GPG key $VAULT_GPGKEY from $server";         gpg --batch --keyserver "$server" --recv-keys "$VAULT_GPGKEY" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $VAULT_GPGKEY" && exit 1;     mkdir -p /tmp/build &&     cd /tmp/build &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS &&     wget https://releases.hashicorp.com/vault/${VAULT_VERSION}/vault_${VAULT_VERSION}_SHA256SUMS.sig &&     gpg --batch --verify vault_${VAULT_VERSION}_SHA256SUMS.sig vault_${VAULT_VERSION}_SHA256SUMS &&     grep vault_${VAULT_VERSION}_linux_${ARCH}.zip vault_${VAULT_VERSION}_SHA256SUMS | sha256sum -c &&     unzip -d /bin vault_${VAULT_VERSION}_linux_${ARCH}.zip &&     cd /tmp &&     rm -rf /tmp/build &&     gpgconf --kill dirmngr &&     gpgconf --kill gpg-agent &&     apk del gnupg openssl &&     rm -rf /root/.gnupg
# Thu, 01 Apr 2021 07:39:09 GMT
# ARGS: VAULT_VERSION=1.7.0
RUN mkdir -p /vault/logs &&     mkdir -p /vault/file &&     mkdir -p /vault/config &&     chown -R vault:vault /vault
# Thu, 01 Apr 2021 07:39:09 GMT
VOLUME [/vault/logs]
# Thu, 01 Apr 2021 07:39:10 GMT
VOLUME [/vault/file]
# Thu, 01 Apr 2021 07:39:10 GMT
EXPOSE 8200
# Thu, 01 Apr 2021 07:39:10 GMT
COPY file:a1e68ac70727f49824592e948e9a677097c8d3752a047b468122ba433b453fc4 in /usr/local/bin/docker-entrypoint.sh 
# Thu, 01 Apr 2021 07:39:10 GMT
ENTRYPOINT ["docker-entrypoint.sh"]
# Thu, 01 Apr 2021 07:39:11 GMT
CMD ["server" "-dev"]
```

-	Layers:
	-	`sha256:b22e590ebf70a9a5901c380b07232ef3c07cb13440402934dfdffb8f8721a949`  
		Last Modified: Wed, 31 Mar 2021 17:44:05 GMT  
		Size: 2.8 MB (2818802 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:253b6fe11e847937b3bb907714a7ba2d39bfe7574e23a0b57a5492261959a9ca`  
		Last Modified: Thu, 01 Apr 2021 07:41:16 GMT  
		Size: 1.3 KB (1257 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76ee58c78adb286aa02cf737f3ef4e76eaaa4501219874cc1b1edd91955ab2e8`  
		Last Modified: Thu, 01 Apr 2021 07:41:29 GMT  
		Size: 67.7 MB (67748638 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bc29516badcc93e7963cd6ac28767a2e3d4cc53aa6da2393e8e786479ef11c41`  
		Last Modified: Thu, 01 Apr 2021 07:41:16 GMT  
		Size: 189.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3e4c24c4948e932b7b5761fe9af854282834a76e1e7d7f24267473911695c8e`  
		Last Modified: Thu, 01 Apr 2021 07:41:16 GMT  
		Size: 1.8 KB (1817 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
