<!-- THIS FILE IS GENERATED VIA './update-remote.sh' -->

# Tags of `eclipse-mosquitto`

-	[`eclipse-mosquitto:1.5`](#eclipse-mosquitto15)
-	[`eclipse-mosquitto:1.5.11`](#eclipse-mosquitto1511)
-	[`eclipse-mosquitto:1.6`](#eclipse-mosquitto16)
-	[`eclipse-mosquitto:1.6-openssl`](#eclipse-mosquitto16-openssl)
-	[`eclipse-mosquitto:1.6.15`](#eclipse-mosquitto1615)
-	[`eclipse-mosquitto:1.6.15-openssl`](#eclipse-mosquitto1615-openssl)
-	[`eclipse-mosquitto:2`](#eclipse-mosquitto2)
-	[`eclipse-mosquitto:2-openssl`](#eclipse-mosquitto2-openssl)
-	[`eclipse-mosquitto:2.0`](#eclipse-mosquitto20)
-	[`eclipse-mosquitto:2.0-openssl`](#eclipse-mosquitto20-openssl)
-	[`eclipse-mosquitto:2.0.11`](#eclipse-mosquitto2011)
-	[`eclipse-mosquitto:2.0.11-openssl`](#eclipse-mosquitto2011-openssl)
-	[`eclipse-mosquitto:latest`](#eclipse-mosquittolatest)
-	[`eclipse-mosquitto:openssl`](#eclipse-mosquittoopenssl)

## `eclipse-mosquitto:1.5`

```console
$ docker pull eclipse-mosquitto@sha256:6c580c5b245c7bba7a6fa793cbaf6d8e165ba190aa761ed1c2223a128ddb3744
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-mosquitto:1.5` - linux; amd64

```console
$ docker pull eclipse-mosquitto@sha256:af602f8fd01f36287b3e3c75e5f688256df5ec2178948a06556b9d11337d6bf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4494289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da9b690585194812e6a57bc3cdab9a90ae244708af5b29e31987d3dae5c8744`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:21:46 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 14 Apr 2021 20:24:08 GMT
ENV VERSION=1.5.11 DOWNLOAD_SHA256=4a3b8a8f5505d27a7a966dd68bfd76f1e69feb51796d1b46b7271d1bb5a1a299 GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=2.4.2 LWS_SHA256=73012d7fcf428dedccc816e83a63a01462e27819d5537b8e0d0c7264bfacfad6
# Thu, 29 Jul 2021 00:24:54 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -flto"         LDFLAGS="-L/build/lws/lib -flto"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes 		WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates 		libressl 		libuuid &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:24:54 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:24:54 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Thu, 29 Jul 2021 00:24:54 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:24:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:24:55 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9198d12407100823c743ef9f96268161990d4539aeb3c815cfc23fac26a1523f`  
		Last Modified: Thu, 29 Jul 2021 00:26:09 GMT  
		Size: 1.7 MB (1693482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9bf8b54f22b1288fa86ed5a0d4440a98abf31de5caefd83065ffc4fe22c7b2`  
		Last Modified: Thu, 29 Jul 2021 00:26:08 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.5` - linux; arm variant v6

```console
$ docker pull eclipse-mosquitto@sha256:296bd04a3ba0a4a3703a08debe93f20f3a319f5e79cf44045dcfca92fb5f0ab5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a78f41da70e0cfdd0c5612f7e88191d350d8ed447fd2841151302dfdfd2bba67`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:51:14 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:56:04 GMT
ENV VERSION=1.5.11 DOWNLOAD_SHA256=4a3b8a8f5505d27a7a966dd68bfd76f1e69feb51796d1b46b7271d1bb5a1a299 GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=2.4.2 LWS_SHA256=73012d7fcf428dedccc816e83a63a01462e27819d5537b8e0d0c7264bfacfad6
# Wed, 28 Jul 2021 23:56:46 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -flto"         LDFLAGS="-L/build/lws/lib -flto"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes 		WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates 		libressl 		libuuid &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:56:46 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:56:47 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:56:47 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:56:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:56:48 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76128bfc4fd19d2af71faa9eaf47ba6c8f77fdfafc7e3dc231d8f53f9dbbdc07`  
		Last Modified: Wed, 28 Jul 2021 23:59:06 GMT  
		Size: 1.6 MB (1552088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884fe0906652bbc7b2da668b2465c8b1f7d0b64e296a5a9084944f2ace8c7742`  
		Last Modified: Wed, 28 Jul 2021 23:59:05 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.5` - linux; arm64 variant v8

```console
$ docker pull eclipse-mosquitto@sha256:f7fd7468d557d0cfa478a9830f948ca504987946ecdd492fc12c6306cc2df8dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4379749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b63dae6f1cae5e908b9ee65d257ff595e30422b200a7d412f1ce5a68e32fdc54`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:33:08 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Tue, 15 Jun 2021 23:35:40 GMT
ENV VERSION=1.5.11 DOWNLOAD_SHA256=4a3b8a8f5505d27a7a966dd68bfd76f1e69feb51796d1b46b7271d1bb5a1a299 GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=2.4.2 LWS_SHA256=73012d7fcf428dedccc816e83a63a01462e27819d5537b8e0d0c7264bfacfad6
# Wed, 28 Jul 2021 23:51:30 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -flto"         LDFLAGS="-L/build/lws/lib -flto"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes 		WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates 		libressl 		libuuid &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:51:30 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:51:30 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:51:31 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:51:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:51:31 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f158ccfd47522703221010f815ac50005809e65d3f050635c3db43b1aaebc06`  
		Last Modified: Wed, 28 Jul 2021 23:53:07 GMT  
		Size: 1.7 MB (1668815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe18ce84c5c4c35ca45f5abb74b6f79a7577039791f7a366d86f8700c67b81fc`  
		Last Modified: Wed, 28 Jul 2021 23:53:06 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.5` - linux; 386

```console
$ docker pull eclipse-mosquitto@sha256:27d44f148748b81456a47a3c99f4038963a66997b39539eb64a8a8f3f791194b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4586354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4104315656f367a88916412dc3b4db672afcc37dc1bd038795307d725a3f5f5c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:38:43 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 14 Apr 2021 23:41:17 GMT
ENV VERSION=1.5.11 DOWNLOAD_SHA256=4a3b8a8f5505d27a7a966dd68bfd76f1e69feb51796d1b46b7271d1bb5a1a299 GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=2.4.2 LWS_SHA256=73012d7fcf428dedccc816e83a63a01462e27819d5537b8e0d0c7264bfacfad6
# Wed, 28 Jul 2021 23:45:41 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -flto"         LDFLAGS="-L/build/lws/lib -flto"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes 		WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates 		libressl 		libuuid &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:45:42 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:45:42 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:45:42 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:45:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:45:43 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b260bbf73cad82fef712d053c3b6c12a3874c47a1ec5523a5e5530fdc792034`  
		Last Modified: Wed, 28 Jul 2021 23:47:26 GMT  
		Size: 1.8 MB (1790321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78b3aee1c69f9210791dafc252749b8a694b6b6628268465864eb9f30f41106`  
		Last Modified: Wed, 28 Jul 2021 23:47:25 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.5` - linux; ppc64le

```console
$ docker pull eclipse-mosquitto@sha256:084008a88033057b71192bb2c61c545ce3f1b9971ddf005365cd93bb71af0c29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4563949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ad3eb78a6079d39b67f921ac2a42116337f3cc35b27135cd4d2428bdec59378`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Thu, 29 Jul 2021 00:23:29 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Thu, 29 Jul 2021 00:31:21 GMT
ENV VERSION=1.5.11 DOWNLOAD_SHA256=4a3b8a8f5505d27a7a966dd68bfd76f1e69feb51796d1b46b7271d1bb5a1a299 GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=2.4.2 LWS_SHA256=73012d7fcf428dedccc816e83a63a01462e27819d5537b8e0d0c7264bfacfad6
# Thu, 29 Jul 2021 00:32:00 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -flto"         LDFLAGS="-L/build/lws/lib -flto"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes 		WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates 		libressl 		libuuid &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:32:04 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:32:07 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Thu, 29 Jul 2021 00:32:12 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:32:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:32:23 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed403aaab3baad440746cf9499436715c71e8a8dded5a97b250a142d200a0fae`  
		Last Modified: Thu, 29 Jul 2021 00:34:08 GMT  
		Size: 1.8 MB (1756961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ad12066da608198121bd98c2daf890dfdf1cb903207add168d6637c58d3fab`  
		Last Modified: Thu, 29 Jul 2021 00:34:08 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.5` - linux; s390x

```console
$ docker pull eclipse-mosquitto@sha256:f8efc7d23f5b9e00c3f419990ff1682843e0d31ef83d797d34a1d431796bafa0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4280724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acdcdd5b18d3b5b9767f04c361a834f828e2fc8b6230d506f2db7d34e1236efd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:46:00 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:48:18 GMT
ENV VERSION=1.5.11 DOWNLOAD_SHA256=4a3b8a8f5505d27a7a966dd68bfd76f1e69feb51796d1b46b7271d1bb5a1a299 GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=2.4.2 LWS_SHA256=73012d7fcf428dedccc816e83a63a01462e27819d5537b8e0d0c7264bfacfad6
# Wed, 28 Jul 2021 23:48:35 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -flto"         LDFLAGS="-L/build/lws/lib -flto"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes 		WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates 		libressl 		libuuid &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:48:35 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:48:35 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:48:36 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:48:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:48:36 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283f21a85615ff899cc9225e51c22bbb47bf32b9a6ad29c19ee76161a7cefd7e`  
		Last Modified: Wed, 28 Jul 2021 23:49:52 GMT  
		Size: 1.7 MB (1712058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd09cecebf5b023bb14dbb9dd5af490f11ccbd2c1786f1c15b836b2a1e08e82`  
		Last Modified: Wed, 28 Jul 2021 23:49:52 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eclipse-mosquitto:1.5.11`

```console
$ docker pull eclipse-mosquitto@sha256:6c580c5b245c7bba7a6fa793cbaf6d8e165ba190aa761ed1c2223a128ddb3744
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-mosquitto:1.5.11` - linux; amd64

```console
$ docker pull eclipse-mosquitto@sha256:af602f8fd01f36287b3e3c75e5f688256df5ec2178948a06556b9d11337d6bf8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4494289 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4da9b690585194812e6a57bc3cdab9a90ae244708af5b29e31987d3dae5c8744`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:21:46 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 14 Apr 2021 20:24:08 GMT
ENV VERSION=1.5.11 DOWNLOAD_SHA256=4a3b8a8f5505d27a7a966dd68bfd76f1e69feb51796d1b46b7271d1bb5a1a299 GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=2.4.2 LWS_SHA256=73012d7fcf428dedccc816e83a63a01462e27819d5537b8e0d0c7264bfacfad6
# Thu, 29 Jul 2021 00:24:54 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -flto"         LDFLAGS="-L/build/lws/lib -flto"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes 		WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates 		libressl 		libuuid &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:24:54 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:24:54 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Thu, 29 Jul 2021 00:24:54 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:24:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:24:55 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9198d12407100823c743ef9f96268161990d4539aeb3c815cfc23fac26a1523f`  
		Last Modified: Thu, 29 Jul 2021 00:26:09 GMT  
		Size: 1.7 MB (1693482 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9bf8b54f22b1288fa86ed5a0d4440a98abf31de5caefd83065ffc4fe22c7b2`  
		Last Modified: Thu, 29 Jul 2021 00:26:08 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.5.11` - linux; arm variant v6

```console
$ docker pull eclipse-mosquitto@sha256:296bd04a3ba0a4a3703a08debe93f20f3a319f5e79cf44045dcfca92fb5f0ab5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.2 MB (4157580 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a78f41da70e0cfdd0c5612f7e88191d350d8ed447fd2841151302dfdfd2bba67`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:51:14 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:56:04 GMT
ENV VERSION=1.5.11 DOWNLOAD_SHA256=4a3b8a8f5505d27a7a966dd68bfd76f1e69feb51796d1b46b7271d1bb5a1a299 GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=2.4.2 LWS_SHA256=73012d7fcf428dedccc816e83a63a01462e27819d5537b8e0d0c7264bfacfad6
# Wed, 28 Jul 2021 23:56:46 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -flto"         LDFLAGS="-L/build/lws/lib -flto"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes 		WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates 		libressl 		libuuid &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:56:46 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:56:47 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:56:47 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:56:48 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:56:48 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:76128bfc4fd19d2af71faa9eaf47ba6c8f77fdfafc7e3dc231d8f53f9dbbdc07`  
		Last Modified: Wed, 28 Jul 2021 23:59:06 GMT  
		Size: 1.6 MB (1552088 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:884fe0906652bbc7b2da668b2465c8b1f7d0b64e296a5a9084944f2ace8c7742`  
		Last Modified: Wed, 28 Jul 2021 23:59:05 GMT  
		Size: 239.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.5.11` - linux; arm64 variant v8

```console
$ docker pull eclipse-mosquitto@sha256:f7fd7468d557d0cfa478a9830f948ca504987946ecdd492fc12c6306cc2df8dd
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4379749 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b63dae6f1cae5e908b9ee65d257ff595e30422b200a7d412f1ce5a68e32fdc54`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:33:08 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Tue, 15 Jun 2021 23:35:40 GMT
ENV VERSION=1.5.11 DOWNLOAD_SHA256=4a3b8a8f5505d27a7a966dd68bfd76f1e69feb51796d1b46b7271d1bb5a1a299 GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=2.4.2 LWS_SHA256=73012d7fcf428dedccc816e83a63a01462e27819d5537b8e0d0c7264bfacfad6
# Wed, 28 Jul 2021 23:51:30 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -flto"         LDFLAGS="-L/build/lws/lib -flto"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes 		WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates 		libressl 		libuuid &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:51:30 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:51:30 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:51:31 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:51:31 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:51:31 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f158ccfd47522703221010f815ac50005809e65d3f050635c3db43b1aaebc06`  
		Last Modified: Wed, 28 Jul 2021 23:53:07 GMT  
		Size: 1.7 MB (1668815 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fe18ce84c5c4c35ca45f5abb74b6f79a7577039791f7a366d86f8700c67b81fc`  
		Last Modified: Wed, 28 Jul 2021 23:53:06 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.5.11` - linux; 386

```console
$ docker pull eclipse-mosquitto@sha256:27d44f148748b81456a47a3c99f4038963a66997b39539eb64a8a8f3f791194b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4586354 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4104315656f367a88916412dc3b4db672afcc37dc1bd038795307d725a3f5f5c`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:38:43 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 14 Apr 2021 23:41:17 GMT
ENV VERSION=1.5.11 DOWNLOAD_SHA256=4a3b8a8f5505d27a7a966dd68bfd76f1e69feb51796d1b46b7271d1bb5a1a299 GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=2.4.2 LWS_SHA256=73012d7fcf428dedccc816e83a63a01462e27819d5537b8e0d0c7264bfacfad6
# Wed, 28 Jul 2021 23:45:41 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -flto"         LDFLAGS="-L/build/lws/lib -flto"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes 		WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates 		libressl 		libuuid &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:45:42 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:45:42 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:45:42 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:45:43 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:45:43 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b260bbf73cad82fef712d053c3b6c12a3874c47a1ec5523a5e5530fdc792034`  
		Last Modified: Wed, 28 Jul 2021 23:47:26 GMT  
		Size: 1.8 MB (1790321 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b78b3aee1c69f9210791dafc252749b8a694b6b6628268465864eb9f30f41106`  
		Last Modified: Wed, 28 Jul 2021 23:47:25 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.5.11` - linux; ppc64le

```console
$ docker pull eclipse-mosquitto@sha256:084008a88033057b71192bb2c61c545ce3f1b9971ddf005365cd93bb71af0c29
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4563949 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6ad3eb78a6079d39b67f921ac2a42116337f3cc35b27135cd4d2428bdec59378`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Thu, 29 Jul 2021 00:23:29 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Thu, 29 Jul 2021 00:31:21 GMT
ENV VERSION=1.5.11 DOWNLOAD_SHA256=4a3b8a8f5505d27a7a966dd68bfd76f1e69feb51796d1b46b7271d1bb5a1a299 GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=2.4.2 LWS_SHA256=73012d7fcf428dedccc816e83a63a01462e27819d5537b8e0d0c7264bfacfad6
# Thu, 29 Jul 2021 00:32:00 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -flto"         LDFLAGS="-L/build/lws/lib -flto"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes 		WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates 		libressl 		libuuid &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:32:04 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:32:07 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Thu, 29 Jul 2021 00:32:12 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:32:17 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:32:23 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed403aaab3baad440746cf9499436715c71e8a8dded5a97b250a142d200a0fae`  
		Last Modified: Thu, 29 Jul 2021 00:34:08 GMT  
		Size: 1.8 MB (1756961 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ad12066da608198121bd98c2daf890dfdf1cb903207add168d6637c58d3fab`  
		Last Modified: Thu, 29 Jul 2021 00:34:08 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.5.11` - linux; s390x

```console
$ docker pull eclipse-mosquitto@sha256:f8efc7d23f5b9e00c3f419990ff1682843e0d31ef83d797d34a1d431796bafa0
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4280724 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:acdcdd5b18d3b5b9767f04c361a834f828e2fc8b6230d506f2db7d34e1236efd`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:46:00 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:48:18 GMT
ENV VERSION=1.5.11 DOWNLOAD_SHA256=4a3b8a8f5505d27a7a966dd68bfd76f1e69feb51796d1b46b7271d1bb5a1a299 GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=2.4.2 LWS_SHA256=73012d7fcf428dedccc816e83a63a01462e27819d5537b8e0d0c7264bfacfad6
# Wed, 28 Jul 2021 23:48:35 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -flto"         LDFLAGS="-L/build/lws/lib -flto"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes 		WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates 		libressl 		libuuid &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:48:35 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:48:35 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:48:36 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:48:36 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:48:36 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:283f21a85615ff899cc9225e51c22bbb47bf32b9a6ad29c19ee76161a7cefd7e`  
		Last Modified: Wed, 28 Jul 2021 23:49:52 GMT  
		Size: 1.7 MB (1712058 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6cd09cecebf5b023bb14dbb9dd5af490f11ccbd2c1786f1c15b836b2a1e08e82`  
		Last Modified: Wed, 28 Jul 2021 23:49:52 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eclipse-mosquitto:1.6`

```console
$ docker pull eclipse-mosquitto@sha256:bb651034dff4f3184e31da66cf6cafb94a58652a577cf23c24bbe599e23cdea4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-mosquitto:1.6` - linux; amd64

```console
$ docker pull eclipse-mosquitto@sha256:a971bd7b5fa449c549f30dab549ea1f4ef4e206b20a3fe1219b2b7dab3ed9a76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4612292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6782fc44234c98db4a7586027047350e25afd947b9d8a32644197c60789d11f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:21:46 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 17:21:23 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Thu, 29 Jul 2021 00:23:54 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:23:54 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:23:54 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Thu, 29 Jul 2021 00:23:55 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:23:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:23:55 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5617a68dd11623e3dc8a901d70df247dca60d4006a67d126b88dc2b041bc5b2`  
		Last Modified: Thu, 29 Jul 2021 00:25:48 GMT  
		Size: 1.8 MB (1811487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39be765cfecfabaf4863e7c8d2cf2e81ced6fb1d94fe3a401d1b88a088942e3e`  
		Last Modified: Thu, 29 Jul 2021 00:25:48 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6` - linux; arm variant v6

```console
$ docker pull eclipse-mosquitto@sha256:d945b9c1cba168526556779e57cc2f16e367c85d327f093b1e267a5fbd7b4db6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4261097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffb00bcb4eeaf3cccad6cdce71ecc61a69381c2e7c78c595fcc05090de567675`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:51:14 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:53:52 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Wed, 28 Jul 2021 23:54:38 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:54:38 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:54:39 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:54:39 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:54:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:54:40 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014ceb5612b6c6180c45386595a71cae064b8d3b1440a17d1d3cecfef47412cd`  
		Last Modified: Wed, 28 Jul 2021 23:58:40 GMT  
		Size: 1.7 MB (1655606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a30e179455f1bd5b2cbe6739b9b34e28c936388fc8d7d668f0c2a0e45f8509`  
		Last Modified: Wed, 28 Jul 2021 23:58:39 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6` - linux; arm64 variant v8

```console
$ docker pull eclipse-mosquitto@sha256:5410f4c079f2f2291e0cd6418cca809877951dd25cb81ebee5dd6da404b12729
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4496570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72373bee80145e5fb6730046fe1138df614ca4138727a19c176abe201ce22289`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:33:08 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Tue, 15 Jun 2021 23:34:36 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Wed, 28 Jul 2021 23:50:30 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:50:30 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:50:30 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:50:30 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:50:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:50:31 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d2b405590e584be6337a69a2122e7fddbb51025d6d09bb82e5d09f1781fe15`  
		Last Modified: Wed, 28 Jul 2021 23:52:44 GMT  
		Size: 1.8 MB (1785636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bd2ddeb3de3d3ec75260e6a261c586625eda7b5dc6f7692348ecc9a6df250a`  
		Last Modified: Wed, 28 Jul 2021 23:52:43 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6` - linux; 386

```console
$ docker pull eclipse-mosquitto@sha256:a71a5434c064d7099d511d484e50b3c4944e962dd028aa517c94bb108ef01aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4715194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a50d308c68303b35971b8d5891ca19e801113a94c9ec8f350a5dda39f71f218`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:38:43 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 18:28:05 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Wed, 28 Jul 2021 23:44:26 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:44:26 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:44:26 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:44:27 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:44:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:44:27 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b60ecd607ed5f3c0f1cecd4eb4f563a57be98e14db24bd3c91678b936a1b9c8`  
		Last Modified: Wed, 28 Jul 2021 23:47:02 GMT  
		Size: 1.9 MB (1919159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43978e01db3ed7872927ddaab1368d801215d7397c7da9d89347c940a32a6e1`  
		Last Modified: Wed, 28 Jul 2021 23:47:01 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6` - linux; ppc64le

```console
$ docker pull eclipse-mosquitto@sha256:4da98b8f979c7fd64f9ad2c421b31fdcecf5e2085a3637bc39d84d01ec8d732b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4701026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b0127a5e0fb90bcde4c359ea3e6704aa863f4a6c55caf2ed2394aa7d5f594f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Thu, 29 Jul 2021 00:23:29 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Thu, 29 Jul 2021 00:27:48 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Thu, 29 Jul 2021 00:28:41 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:28:52 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:28:59 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Thu, 29 Jul 2021 00:29:10 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:29:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:29:28 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ad88d11c1a540d9896c913f4c9b5ebebda9f41640106f46eedc8b1a977b557`  
		Last Modified: Thu, 29 Jul 2021 00:33:46 GMT  
		Size: 1.9 MB (1894038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a150d7e79eeb66e9990abb2dfe4b2292a02182be38e3230ac744bbef71c0bf3`  
		Last Modified: Thu, 29 Jul 2021 00:33:45 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6` - linux; s390x

```console
$ docker pull eclipse-mosquitto@sha256:fcf59b31a544465f4e2d42735b5821717d6b3613f253852a2b42c0c6292a62af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4396005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3090a5fbc6dd96e027506e4867f7cae04ed4f64a47efff625ea1d9676b359f05`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:46:00 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:47:20 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Wed, 28 Jul 2021 23:47:40 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:47:40 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:47:40 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:47:40 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:47:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:47:41 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16aad7570810b133aa4642232b728998d30f955704df47d97ab12affe1c6cb7`  
		Last Modified: Wed, 28 Jul 2021 23:49:37 GMT  
		Size: 1.8 MB (1827339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518e75f72bb3715fee4e557f637e80d8bf490f84c08185a28d3fffcb6c912868`  
		Last Modified: Wed, 28 Jul 2021 23:49:37 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eclipse-mosquitto:1.6-openssl`

```console
$ docker pull eclipse-mosquitto@sha256:b58dc08aaa86e753f79f4c50a99fdf4981309a92817a51206fc83de739553d08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-mosquitto:1.6-openssl` - linux; amd64

```console
$ docker pull eclipse-mosquitto@sha256:276ff1376d74a3b5b13537bdf731c6e84eef52dddfa0e8c2a9860ca066a31dba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3425672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38972d3e57ba52011e5d9ce832e89522ad3149ab4f6c6245b46caef029a534c4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:21:46 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 17:21:23 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Thu, 29 Jul 2021 00:24:27 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:24:27 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:24:27 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Thu, 29 Jul 2021 00:24:27 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:24:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:24:28 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5920877403127325edd4375554b61f18084ebdf9210f70820a0a750211851e90`  
		Last Modified: Thu, 29 Jul 2021 00:25:58 GMT  
		Size: 624.9 KB (624867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5fa32e4f82787bb85d0ada1222d2d789a403b1a9b3edfb9cf1484dbf1a8422`  
		Last Modified: Thu, 29 Jul 2021 00:25:58 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6-openssl` - linux; arm variant v6

```console
$ docker pull eclipse-mosquitto@sha256:74805ee4269fb5b69ac3181fb4bdaacf5be6278039765a07160d90e6c239b968
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3198305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:183bd84a8d361251e8a7eead77518b6effe1cf43a6be341e5aca05ebffdcf068`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:51:14 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:53:52 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Wed, 28 Jul 2021 23:55:44 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:55:44 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:55:45 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:55:45 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:55:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:55:46 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808d3fc7d96e96dd32e278625b186caa146073d8fb9b127eb18b89f90abdad8f`  
		Last Modified: Wed, 28 Jul 2021 23:58:53 GMT  
		Size: 592.8 KB (592814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f824352f96ca4f41c490d64c23000814b4bda8ae6b278941c9641fd47a5325dd`  
		Last Modified: Wed, 28 Jul 2021 23:58:52 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6-openssl` - linux; arm64 variant v8

```console
$ docker pull eclipse-mosquitto@sha256:33bc9f6c2adb2c0b301998fbd4486f0d49d1feb1a07aeec3778209f99e90b53e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3333624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38cc722c6ad55fcf8ff03a7ea5f88108bd578ee3c8c98e6136a2bcff7f5a98f0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:33:08 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Tue, 15 Jun 2021 23:34:36 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Wed, 28 Jul 2021 23:51:03 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:51:03 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:51:03 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:51:03 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:51:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:51:04 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318015ba6cee7917df87e170ff3fba66fabd23a05c892be357c543426f101390`  
		Last Modified: Wed, 28 Jul 2021 23:52:55 GMT  
		Size: 622.7 KB (622692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f478d48b9e3c1e885017a7476a93bf33b6517c8cc113e498ea4372608e20e262`  
		Last Modified: Wed, 28 Jul 2021 23:52:55 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6-openssl` - linux; 386

```console
$ docker pull eclipse-mosquitto@sha256:8842a3652760dd148587e6d9c558a0d88c071428e8abf8d4397b3b2d32956aca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3444709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2216dc2b8adf3692c1db3a514ba7cc4c38f8423fa0c0cb6cda69c5d89d8b0aa9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:38:43 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 18:28:05 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Wed, 28 Jul 2021 23:45:05 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:45:05 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:45:06 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:45:06 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:45:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:45:06 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58390a3dae57bf0795f4758d93cfeb6e39b0a8a8ed0d1dc37ed1691ca3616414`  
		Last Modified: Wed, 28 Jul 2021 23:47:13 GMT  
		Size: 648.7 KB (648674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bac8023e6383a135b4870072749eb794f2ef7b4a7387489931c14aaaa91f97`  
		Last Modified: Wed, 28 Jul 2021 23:47:13 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6-openssl` - linux; ppc64le

```console
$ docker pull eclipse-mosquitto@sha256:9d6901d042b29f2bb30f91d1875a4b9ca256665ee0b7be3659ee3a37bd424eec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3482527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44c1e0a01cb02f9c69b4a3828b61662082eabc681f5057b16afa0fccad63a26f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Thu, 29 Jul 2021 00:23:29 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Thu, 29 Jul 2021 00:27:48 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Thu, 29 Jul 2021 00:30:26 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:30:34 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:30:38 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Thu, 29 Jul 2021 00:30:43 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:30:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:31:01 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ff904607bf8a17639794336bf022179634f5504e3866490fb69e4f04b86698`  
		Last Modified: Thu, 29 Jul 2021 00:33:57 GMT  
		Size: 675.5 KB (675540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176727b1e6843d058578a5524e65bf34c198bfd3dff8c65f1c7a2021b3cbcdcf`  
		Last Modified: Thu, 29 Jul 2021 00:33:57 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6-openssl` - linux; s390x

```console
$ docker pull eclipse-mosquitto@sha256:f9ceedde0176f340d7fad8bc902ad0fd6c171ae93a547ec27badbe4ba90306c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3185733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600362f792e33d373240a0030c2258848ddc002fe4bf31efa50af6b9a756b712`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:46:00 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:47:20 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Wed, 28 Jul 2021 23:48:08 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:48:08 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:48:09 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:48:09 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:48:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:48:09 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42f0c002547277f40399b41e70cb93f87cc1697c570186a0871123bc0e13313`  
		Last Modified: Wed, 28 Jul 2021 23:49:45 GMT  
		Size: 617.1 KB (617067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0815d150b5db8c5c7f014b00bfd48afb7f19600dc9b0935711409f3dfb3f9590`  
		Last Modified: Wed, 28 Jul 2021 23:49:44 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eclipse-mosquitto:1.6.15`

```console
$ docker pull eclipse-mosquitto@sha256:bb651034dff4f3184e31da66cf6cafb94a58652a577cf23c24bbe599e23cdea4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-mosquitto:1.6.15` - linux; amd64

```console
$ docker pull eclipse-mosquitto@sha256:a971bd7b5fa449c549f30dab549ea1f4ef4e206b20a3fe1219b2b7dab3ed9a76
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4612292 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e6782fc44234c98db4a7586027047350e25afd947b9d8a32644197c60789d11f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:21:46 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 17:21:23 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Thu, 29 Jul 2021 00:23:54 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:23:54 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:23:54 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Thu, 29 Jul 2021 00:23:55 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:23:55 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:23:55 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c5617a68dd11623e3dc8a901d70df247dca60d4006a67d126b88dc2b041bc5b2`  
		Last Modified: Thu, 29 Jul 2021 00:25:48 GMT  
		Size: 1.8 MB (1811487 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:39be765cfecfabaf4863e7c8d2cf2e81ced6fb1d94fe3a401d1b88a088942e3e`  
		Last Modified: Thu, 29 Jul 2021 00:25:48 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6.15` - linux; arm variant v6

```console
$ docker pull eclipse-mosquitto@sha256:d945b9c1cba168526556779e57cc2f16e367c85d327f093b1e267a5fbd7b4db6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.3 MB (4261097 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ffb00bcb4eeaf3cccad6cdce71ecc61a69381c2e7c78c595fcc05090de567675`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:51:14 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:53:52 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Wed, 28 Jul 2021 23:54:38 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:54:38 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:54:39 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:54:39 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:54:40 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:54:40 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:014ceb5612b6c6180c45386595a71cae064b8d3b1440a17d1d3cecfef47412cd`  
		Last Modified: Wed, 28 Jul 2021 23:58:40 GMT  
		Size: 1.7 MB (1655606 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4a30e179455f1bd5b2cbe6739b9b34e28c936388fc8d7d668f0c2a0e45f8509`  
		Last Modified: Wed, 28 Jul 2021 23:58:39 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6.15` - linux; arm64 variant v8

```console
$ docker pull eclipse-mosquitto@sha256:5410f4c079f2f2291e0cd6418cca809877951dd25cb81ebee5dd6da404b12729
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4496570 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:72373bee80145e5fb6730046fe1138df614ca4138727a19c176abe201ce22289`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:33:08 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Tue, 15 Jun 2021 23:34:36 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Wed, 28 Jul 2021 23:50:30 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:50:30 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:50:30 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:50:30 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:50:30 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:50:31 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:87d2b405590e584be6337a69a2122e7fddbb51025d6d09bb82e5d09f1781fe15`  
		Last Modified: Wed, 28 Jul 2021 23:52:44 GMT  
		Size: 1.8 MB (1785636 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2bd2ddeb3de3d3ec75260e6a261c586625eda7b5dc6f7692348ecc9a6df250a`  
		Last Modified: Wed, 28 Jul 2021 23:52:43 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6.15` - linux; 386

```console
$ docker pull eclipse-mosquitto@sha256:a71a5434c064d7099d511d484e50b3c4944e962dd028aa517c94bb108ef01aab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4715194 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:5a50d308c68303b35971b8d5891ca19e801113a94c9ec8f350a5dda39f71f218`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:38:43 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 18:28:05 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Wed, 28 Jul 2021 23:44:26 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:44:26 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:44:26 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:44:27 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:44:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:44:27 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b60ecd607ed5f3c0f1cecd4eb4f563a57be98e14db24bd3c91678b936a1b9c8`  
		Last Modified: Wed, 28 Jul 2021 23:47:02 GMT  
		Size: 1.9 MB (1919159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c43978e01db3ed7872927ddaab1368d801215d7397c7da9d89347c940a32a6e1`  
		Last Modified: Wed, 28 Jul 2021 23:47:01 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6.15` - linux; ppc64le

```console
$ docker pull eclipse-mosquitto@sha256:4da98b8f979c7fd64f9ad2c421b31fdcecf5e2085a3637bc39d84d01ec8d732b
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4701026 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:13b0127a5e0fb90bcde4c359ea3e6704aa863f4a6c55caf2ed2394aa7d5f594f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Thu, 29 Jul 2021 00:23:29 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Thu, 29 Jul 2021 00:27:48 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Thu, 29 Jul 2021 00:28:41 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:28:52 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:28:59 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Thu, 29 Jul 2021 00:29:10 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:29:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:29:28 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:02ad88d11c1a540d9896c913f4c9b5ebebda9f41640106f46eedc8b1a977b557`  
		Last Modified: Thu, 29 Jul 2021 00:33:46 GMT  
		Size: 1.9 MB (1894038 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8a150d7e79eeb66e9990abb2dfe4b2292a02182be38e3230ac744bbef71c0bf3`  
		Last Modified: Thu, 29 Jul 2021 00:33:45 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6.15` - linux; s390x

```console
$ docker pull eclipse-mosquitto@sha256:fcf59b31a544465f4e2d42735b5821717d6b3613f253852a2b42c0c6292a62af
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4396005 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3090a5fbc6dd96e027506e4867f7cae04ed4f64a47efff625ea1d9676b359f05`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:46:00 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:47:20 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Wed, 28 Jul 2021 23:47:40 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:47:40 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:47:40 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:47:40 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:47:41 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:47:41 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c16aad7570810b133aa4642232b728998d30f955704df47d97ab12affe1c6cb7`  
		Last Modified: Wed, 28 Jul 2021 23:49:37 GMT  
		Size: 1.8 MB (1827339 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:518e75f72bb3715fee4e557f637e80d8bf490f84c08185a28d3fffcb6c912868`  
		Last Modified: Wed, 28 Jul 2021 23:49:37 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eclipse-mosquitto:1.6.15-openssl`

```console
$ docker pull eclipse-mosquitto@sha256:b58dc08aaa86e753f79f4c50a99fdf4981309a92817a51206fc83de739553d08
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-mosquitto:1.6.15-openssl` - linux; amd64

```console
$ docker pull eclipse-mosquitto@sha256:276ff1376d74a3b5b13537bdf731c6e84eef52dddfa0e8c2a9860ca066a31dba
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3425672 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38972d3e57ba52011e5d9ce832e89522ad3149ab4f6c6245b46caef029a534c4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:21:46 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 17:21:23 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Thu, 29 Jul 2021 00:24:27 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:24:27 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:24:27 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Thu, 29 Jul 2021 00:24:27 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:24:27 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:24:28 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5920877403127325edd4375554b61f18084ebdf9210f70820a0a750211851e90`  
		Last Modified: Thu, 29 Jul 2021 00:25:58 GMT  
		Size: 624.9 KB (624867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f5fa32e4f82787bb85d0ada1222d2d789a403b1a9b3edfb9cf1484dbf1a8422`  
		Last Modified: Thu, 29 Jul 2021 00:25:58 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6.15-openssl` - linux; arm variant v6

```console
$ docker pull eclipse-mosquitto@sha256:74805ee4269fb5b69ac3181fb4bdaacf5be6278039765a07160d90e6c239b968
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3198305 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:183bd84a8d361251e8a7eead77518b6effe1cf43a6be341e5aca05ebffdcf068`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:51:14 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:53:52 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Wed, 28 Jul 2021 23:55:44 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:55:44 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:55:45 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:55:45 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:55:46 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:55:46 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:808d3fc7d96e96dd32e278625b186caa146073d8fb9b127eb18b89f90abdad8f`  
		Last Modified: Wed, 28 Jul 2021 23:58:53 GMT  
		Size: 592.8 KB (592814 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f824352f96ca4f41c490d64c23000814b4bda8ae6b278941c9641fd47a5325dd`  
		Last Modified: Wed, 28 Jul 2021 23:58:52 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6.15-openssl` - linux; arm64 variant v8

```console
$ docker pull eclipse-mosquitto@sha256:33bc9f6c2adb2c0b301998fbd4486f0d49d1feb1a07aeec3778209f99e90b53e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3333624 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:38cc722c6ad55fcf8ff03a7ea5f88108bd578ee3c8c98e6136a2bcff7f5a98f0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:33:08 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Tue, 15 Jun 2021 23:34:36 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Wed, 28 Jul 2021 23:51:03 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:51:03 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:51:03 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:51:03 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:51:03 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:51:04 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:318015ba6cee7917df87e170ff3fba66fabd23a05c892be357c543426f101390`  
		Last Modified: Wed, 28 Jul 2021 23:52:55 GMT  
		Size: 622.7 KB (622692 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f478d48b9e3c1e885017a7476a93bf33b6517c8cc113e498ea4372608e20e262`  
		Last Modified: Wed, 28 Jul 2021 23:52:55 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6.15-openssl` - linux; 386

```console
$ docker pull eclipse-mosquitto@sha256:8842a3652760dd148587e6d9c558a0d88c071428e8abf8d4397b3b2d32956aca
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.4 MB (3444709 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2216dc2b8adf3692c1db3a514ba7cc4c38f8423fa0c0cb6cda69c5d89d8b0aa9`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:38:43 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 18:28:05 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Wed, 28 Jul 2021 23:45:05 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:45:05 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:45:06 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:45:06 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:45:06 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:45:06 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:58390a3dae57bf0795f4758d93cfeb6e39b0a8a8ed0d1dc37ed1691ca3616414`  
		Last Modified: Wed, 28 Jul 2021 23:47:13 GMT  
		Size: 648.7 KB (648674 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c3bac8023e6383a135b4870072749eb794f2ef7b4a7387489931c14aaaa91f97`  
		Last Modified: Wed, 28 Jul 2021 23:47:13 GMT  
		Size: 240.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6.15-openssl` - linux; ppc64le

```console
$ docker pull eclipse-mosquitto@sha256:9d6901d042b29f2bb30f91d1875a4b9ca256665ee0b7be3659ee3a37bd424eec
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3482527 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:44c1e0a01cb02f9c69b4a3828b61662082eabc681f5057b16afa0fccad63a26f`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Thu, 29 Jul 2021 00:23:29 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Thu, 29 Jul 2021 00:27:48 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Thu, 29 Jul 2021 00:30:26 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:30:34 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:30:38 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Thu, 29 Jul 2021 00:30:43 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:30:56 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:31:01 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91ff904607bf8a17639794336bf022179634f5504e3866490fb69e4f04b86698`  
		Last Modified: Thu, 29 Jul 2021 00:33:57 GMT  
		Size: 675.5 KB (675540 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:176727b1e6843d058578a5524e65bf34c198bfd3dff8c65f1c7a2021b3cbcdcf`  
		Last Modified: Thu, 29 Jul 2021 00:33:57 GMT  
		Size: 237.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:1.6.15-openssl` - linux; s390x

```console
$ docker pull eclipse-mosquitto@sha256:f9ceedde0176f340d7fad8bc902ad0fd6c171ae93a547ec27badbe4ba90306c8
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.2 MB (3185733 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:600362f792e33d373240a0030c2258848ddc002fe4bf31efa50af6b9a756b712`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:46:00 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:47:20 GMT
ENV VERSION=1.6.15 DOWNLOAD_SHA256=5ff2271512f745bf1a451072cd3768a5daed71e90c5179fae12b049d6c02aa0f GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40
# Wed, 28 Jul 2021 23:48:08 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include"         LDFLAGS="-L/build/lws/lib"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/src/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v10 /usr/share/licenses/mosquitto/epl-v10 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:48:08 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:48:09 GMT
COPY file:232de3a06de79606b9743327f59defda56818d50c1027dd2f0f1c5fb7917db2e in / 
# Wed, 28 Jul 2021 23:48:09 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:48:09 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:48:09 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d42f0c002547277f40399b41e70cb93f87cc1697c570186a0871123bc0e13313`  
		Last Modified: Wed, 28 Jul 2021 23:49:45 GMT  
		Size: 617.1 KB (617067 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0815d150b5db8c5c7f014b00bfd48afb7f19600dc9b0935711409f3dfb3f9590`  
		Last Modified: Wed, 28 Jul 2021 23:49:44 GMT  
		Size: 238.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eclipse-mosquitto:2`

```console
$ docker pull eclipse-mosquitto@sha256:8f80383b4c14b6fcfbfb23b7d6014b6c7fc7ef9c3f7d6ae8fd12d286d81acc46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-mosquitto:2` - linux; amd64

```console
$ docker pull eclipse-mosquitto@sha256:610eaf4aadce8090d4a6af580788189272ca9ba39671cd9ab02f47df9ed0461e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4733862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a8baae5c3fc5eb59fa173f9acc042c276fc204e371b834b7b32326f2197480`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:21:46 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 17:19:41 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Thu, 29 Jul 2021 00:22:34 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:22:34 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:22:34 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Thu, 29 Jul 2021 00:22:35 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:22:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:22:35 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c621ea1b2e689a87634043f08d91fe28277b1024847ba4d2ddac287c36e147`  
		Last Modified: Thu, 29 Jul 2021 00:25:18 GMT  
		Size: 1.9 MB (1932927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5a90f7f9abbe83f31858a296b8ac2347ae474d982c30c6c78a363432d16420`  
		Last Modified: Thu, 29 Jul 2021 00:25:17 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2` - linux; arm variant v6

```console
$ docker pull eclipse-mosquitto@sha256:efbb43243a562aa47fbba37e3d71be61d2ff78c035b84913324ca7a281cd23c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4376622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0118196891ad1173e90238ddc67e90cd805c5fb0333d37f52b6ed94119cb93bb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:51:14 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:51:14 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:52:17 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:52:18 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:52:19 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:52:19 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:52:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:52:20 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfa3e90898f09f982660e08d7d057e186d0da403ba25b059f991cdec11d1620`  
		Last Modified: Wed, 28 Jul 2021 23:58:00 GMT  
		Size: 1.8 MB (1771001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc49daa6fb8480af875b9239c9f282479d6c88ac6c613ed39d8c94110420779`  
		Last Modified: Wed, 28 Jul 2021 23:58:00 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2` - linux; arm64 variant v8

```console
$ docker pull eclipse-mosquitto@sha256:42e95a9a11914eba10106bb7d2b8be09d2416f20bf602a244615201c2d63b700
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4617441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cfb93cbd7e20c634f535c8b2ec3e67a51332a25a17f1de08cd8fe46e0cdcb85`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:33:08 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Tue, 15 Jun 2021 23:33:08 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:49:15 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:49:15 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:49:15 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:49:15 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:49:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:49:16 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf6e679922572c915d192412351500f438150c207acd6dae70a25c94a85dfb9`  
		Last Modified: Wed, 28 Jul 2021 23:52:09 GMT  
		Size: 1.9 MB (1906379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a310f4cbd62b3af8de7f3e77c7ecde0525b23ff5e07888b48e324f8c06aacf94`  
		Last Modified: Wed, 28 Jul 2021 23:52:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2` - linux; 386

```console
$ docker pull eclipse-mosquitto@sha256:3612394bbc5ac0d52f091bb368e821d89e691082bf16e3eb5ebcfaf557318016
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4847770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:083368fe7e4f2a2c24bcab9cfb488bae1ff09c107a34988515e65b6ada996e8b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:38:43 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 18:25:50 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:42:43 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:42:43 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:42:44 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:42:44 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:42:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:42:44 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51797827808a88c53d628823b4ecbd55c66d931e48c2262e4d2356c08f1052a`  
		Last Modified: Wed, 28 Jul 2021 23:46:25 GMT  
		Size: 2.1 MB (2051608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe73ed5d711a9a6f334bc5e0459bd82b9f86d04900dd2310348ec7813ee3707`  
		Last Modified: Wed, 28 Jul 2021 23:46:24 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2` - linux; ppc64le

```console
$ docker pull eclipse-mosquitto@sha256:a339579b235aaf7224551ba16f739c585e12e99c9a9dc40b4f1d5d39ce8b1dab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4846083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f83924be6138538b0f5fd17f69726095075c336aeb0fab2e0381d1a618d59bc4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Thu, 29 Jul 2021 00:23:29 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Thu, 29 Jul 2021 00:23:37 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Thu, 29 Jul 2021 00:24:45 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:24:56 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:24:59 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Thu, 29 Jul 2021 00:25:05 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:25:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:25:20 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4778c7030906a8e96907db2897a87a9674b97e78edaff18b1c934eece90ef4`  
		Last Modified: Thu, 29 Jul 2021 00:33:10 GMT  
		Size: 2.0 MB (2038966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674bebb6c7890560f8749875d7964eb35130983172bed3cbbd9335b86eb23f1a`  
		Last Modified: Thu, 29 Jul 2021 00:33:09 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2` - linux; s390x

```console
$ docker pull eclipse-mosquitto@sha256:d5a2274bf3061aeee30c0d48dc42bad0389919f1db755cb2b6143c7eaf8271e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4518101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f7a06b56186bb8148b90ffcd305cccab9102df332ecb1c29a425e52dd066e3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:46:00 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:46:00 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:46:33 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:46:33 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:46:33 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:46:34 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:46:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:46:34 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e5e08ac493722d7e19825df6caeab115dcec2dcb207fb5d7981c511163c5e4`  
		Last Modified: Wed, 28 Jul 2021 23:49:16 GMT  
		Size: 1.9 MB (1949305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c409893653081bff1b92986bf8bd505c059b445d8014c545a4e7bdb12ca006a1`  
		Last Modified: Wed, 28 Jul 2021 23:49:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eclipse-mosquitto:2-openssl`

```console
$ docker pull eclipse-mosquitto@sha256:3d83387a181d1a8e5a1f14bbb2b36d695d33acbcfed55c60fb6f75c4de5f13d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-mosquitto:2-openssl` - linux; amd64

```console
$ docker pull eclipse-mosquitto@sha256:de5c92f91918beb14133e1c5c2bc2f88096d28124e4b2f007c8d67cb9ad98df6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3548802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b658f2c808c9d64c61e43a04d3f7dc3fbc72da473f31e06b7838762a634c027`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:21:46 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 17:19:41 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Thu, 29 Jul 2021 00:23:24 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:23:24 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:23:24 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Thu, 29 Jul 2021 00:23:24 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:23:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:23:25 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c80b8bd2d83c8acb5fcaa6d64fec6f5d3d294d46f1567976afee5ba240a0d6`  
		Last Modified: Thu, 29 Jul 2021 00:25:33 GMT  
		Size: 747.9 KB (747867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d2714621edf634a2bfe5474f4a391445dde2a9fbc5252cd393f421f73ee755`  
		Last Modified: Thu, 29 Jul 2021 00:25:32 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2-openssl` - linux; arm variant v6

```console
$ docker pull eclipse-mosquitto@sha256:db52d87d2c4eb6386811d96f5dbe1a2c78e1f46df8a1d48fdf4b78c86dd0262f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3313989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:664e1b21126264b0b045dbc7cdbfe28f9af81f1b8b69386775738650dbaf615e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:51:14 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:51:14 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:53:36 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:53:36 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:53:37 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:53:37 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:53:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:53:38 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ccb38e36f37ca6646fb20a7cdb1b2a5b7e147064198abc051f661711d9800`  
		Last Modified: Wed, 28 Jul 2021 23:58:20 GMT  
		Size: 708.4 KB (708369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d77c03049a432ecb5029af93e3a92a230cce4513c13633d843f634a9ee68ea5`  
		Last Modified: Wed, 28 Jul 2021 23:58:20 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2-openssl` - linux; arm64 variant v8

```console
$ docker pull eclipse-mosquitto@sha256:56669361c3ce0cba5da58075d399f2a1f3dbc1d71d50f44715ce0c8fea96b746
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3454751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d487ad59fd2c73679cd52f9291c36625b26e440cc74a1a83b55dd5ea65cb7ff`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:33:08 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Tue, 15 Jun 2021 23:33:08 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:49:59 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:49:59 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:49:59 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:49:59 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:49:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:50:00 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75ec133029338b56c30de97bb847ca01bfb16aebc0ff5c576e9ab900a4364b8`  
		Last Modified: Wed, 28 Jul 2021 23:52:27 GMT  
		Size: 743.7 KB (743689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5e61cfd4deb3d00131ec56368c51781e579e550ead1242ba84dbbf868e5421`  
		Last Modified: Wed, 28 Jul 2021 23:52:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2-openssl` - linux; 386

```console
$ docker pull eclipse-mosquitto@sha256:78ebe2cbd2a1265f008c405041587c4d3063c5ab1dec755b876227002ef2dc1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3575739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6775b7c456948e0455209005da7c2c0d85a82807dc8fdd0b1530ee3b7234f7e2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:38:43 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 18:25:50 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:43:41 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:43:41 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:43:42 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:43:42 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:43:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:43:43 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d70dba08366c843b421aa6ed16675ea19159ec167a740b6d498ce618bd48972`  
		Last Modified: Wed, 28 Jul 2021 23:46:43 GMT  
		Size: 779.6 KB (779577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2b828537676a2beb7525de65a180944e17c9ecb16055fc2344957b95011c27`  
		Last Modified: Wed, 28 Jul 2021 23:46:43 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2-openssl` - linux; ppc64le

```console
$ docker pull eclipse-mosquitto@sha256:369cf5d4e988adff6b57b4d684109616abe6bdb1f99c5f93b497572d9fcc2213
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3627887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb9702fc0f39ed65d1e770bacf7b03009b0c6ac0dd6d11a15584bb0e1b49c0a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Thu, 29 Jul 2021 00:23:29 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Thu, 29 Jul 2021 00:23:37 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Thu, 29 Jul 2021 00:26:36 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:26:46 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:26:53 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Thu, 29 Jul 2021 00:27:05 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:27:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:27:24 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f894f1cd17c1894dd8edbf22593f163ca65075b8cc46dc10013bf5d5dc2991`  
		Last Modified: Thu, 29 Jul 2021 00:33:28 GMT  
		Size: 820.8 KB (820769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f6feee539bd2ca5bdeb92ca6757e5ce9faae07c52f9f05fc4a9661bedecd38`  
		Last Modified: Thu, 29 Jul 2021 00:33:27 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2-openssl` - linux; s390x

```console
$ docker pull eclipse-mosquitto@sha256:dec6a71c656ca265bfc82be5abb61a2d7e61c6eb621d394aef4c8355e677834c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3307538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:080b10312d76f275fa738e7f2b07479dd610fcb30632de1e62eeba77c059b6a0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:46:00 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:46:00 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:47:11 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:47:11 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:47:12 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:47:12 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:47:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:47:12 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081619879b747e9d716c5dcbb56fce0ea44dda274ccfcd25a63f6d639bcbe067`  
		Last Modified: Wed, 28 Jul 2021 23:49:27 GMT  
		Size: 738.7 KB (738742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03aa253a5b6b699f75c7a54a0205d8fd44fdff9b3d35c89e80789e6bb0af8432`  
		Last Modified: Wed, 28 Jul 2021 23:49:27 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eclipse-mosquitto:2.0`

```console
$ docker pull eclipse-mosquitto@sha256:8f80383b4c14b6fcfbfb23b7d6014b6c7fc7ef9c3f7d6ae8fd12d286d81acc46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-mosquitto:2.0` - linux; amd64

```console
$ docker pull eclipse-mosquitto@sha256:610eaf4aadce8090d4a6af580788189272ca9ba39671cd9ab02f47df9ed0461e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4733862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a8baae5c3fc5eb59fa173f9acc042c276fc204e371b834b7b32326f2197480`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:21:46 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 17:19:41 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Thu, 29 Jul 2021 00:22:34 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:22:34 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:22:34 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Thu, 29 Jul 2021 00:22:35 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:22:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:22:35 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c621ea1b2e689a87634043f08d91fe28277b1024847ba4d2ddac287c36e147`  
		Last Modified: Thu, 29 Jul 2021 00:25:18 GMT  
		Size: 1.9 MB (1932927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5a90f7f9abbe83f31858a296b8ac2347ae474d982c30c6c78a363432d16420`  
		Last Modified: Thu, 29 Jul 2021 00:25:17 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0` - linux; arm variant v6

```console
$ docker pull eclipse-mosquitto@sha256:efbb43243a562aa47fbba37e3d71be61d2ff78c035b84913324ca7a281cd23c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4376622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0118196891ad1173e90238ddc67e90cd805c5fb0333d37f52b6ed94119cb93bb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:51:14 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:51:14 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:52:17 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:52:18 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:52:19 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:52:19 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:52:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:52:20 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfa3e90898f09f982660e08d7d057e186d0da403ba25b059f991cdec11d1620`  
		Last Modified: Wed, 28 Jul 2021 23:58:00 GMT  
		Size: 1.8 MB (1771001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc49daa6fb8480af875b9239c9f282479d6c88ac6c613ed39d8c94110420779`  
		Last Modified: Wed, 28 Jul 2021 23:58:00 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0` - linux; arm64 variant v8

```console
$ docker pull eclipse-mosquitto@sha256:42e95a9a11914eba10106bb7d2b8be09d2416f20bf602a244615201c2d63b700
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4617441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cfb93cbd7e20c634f535c8b2ec3e67a51332a25a17f1de08cd8fe46e0cdcb85`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:33:08 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Tue, 15 Jun 2021 23:33:08 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:49:15 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:49:15 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:49:15 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:49:15 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:49:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:49:16 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf6e679922572c915d192412351500f438150c207acd6dae70a25c94a85dfb9`  
		Last Modified: Wed, 28 Jul 2021 23:52:09 GMT  
		Size: 1.9 MB (1906379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a310f4cbd62b3af8de7f3e77c7ecde0525b23ff5e07888b48e324f8c06aacf94`  
		Last Modified: Wed, 28 Jul 2021 23:52:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0` - linux; 386

```console
$ docker pull eclipse-mosquitto@sha256:3612394bbc5ac0d52f091bb368e821d89e691082bf16e3eb5ebcfaf557318016
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4847770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:083368fe7e4f2a2c24bcab9cfb488bae1ff09c107a34988515e65b6ada996e8b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:38:43 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 18:25:50 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:42:43 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:42:43 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:42:44 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:42:44 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:42:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:42:44 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51797827808a88c53d628823b4ecbd55c66d931e48c2262e4d2356c08f1052a`  
		Last Modified: Wed, 28 Jul 2021 23:46:25 GMT  
		Size: 2.1 MB (2051608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe73ed5d711a9a6f334bc5e0459bd82b9f86d04900dd2310348ec7813ee3707`  
		Last Modified: Wed, 28 Jul 2021 23:46:24 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0` - linux; ppc64le

```console
$ docker pull eclipse-mosquitto@sha256:a339579b235aaf7224551ba16f739c585e12e99c9a9dc40b4f1d5d39ce8b1dab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4846083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f83924be6138538b0f5fd17f69726095075c336aeb0fab2e0381d1a618d59bc4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Thu, 29 Jul 2021 00:23:29 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Thu, 29 Jul 2021 00:23:37 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Thu, 29 Jul 2021 00:24:45 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:24:56 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:24:59 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Thu, 29 Jul 2021 00:25:05 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:25:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:25:20 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4778c7030906a8e96907db2897a87a9674b97e78edaff18b1c934eece90ef4`  
		Last Modified: Thu, 29 Jul 2021 00:33:10 GMT  
		Size: 2.0 MB (2038966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674bebb6c7890560f8749875d7964eb35130983172bed3cbbd9335b86eb23f1a`  
		Last Modified: Thu, 29 Jul 2021 00:33:09 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0` - linux; s390x

```console
$ docker pull eclipse-mosquitto@sha256:d5a2274bf3061aeee30c0d48dc42bad0389919f1db755cb2b6143c7eaf8271e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4518101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f7a06b56186bb8148b90ffcd305cccab9102df332ecb1c29a425e52dd066e3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:46:00 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:46:00 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:46:33 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:46:33 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:46:33 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:46:34 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:46:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:46:34 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e5e08ac493722d7e19825df6caeab115dcec2dcb207fb5d7981c511163c5e4`  
		Last Modified: Wed, 28 Jul 2021 23:49:16 GMT  
		Size: 1.9 MB (1949305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c409893653081bff1b92986bf8bd505c059b445d8014c545a4e7bdb12ca006a1`  
		Last Modified: Wed, 28 Jul 2021 23:49:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eclipse-mosquitto:2.0-openssl`

```console
$ docker pull eclipse-mosquitto@sha256:3d83387a181d1a8e5a1f14bbb2b36d695d33acbcfed55c60fb6f75c4de5f13d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-mosquitto:2.0-openssl` - linux; amd64

```console
$ docker pull eclipse-mosquitto@sha256:de5c92f91918beb14133e1c5c2bc2f88096d28124e4b2f007c8d67cb9ad98df6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3548802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b658f2c808c9d64c61e43a04d3f7dc3fbc72da473f31e06b7838762a634c027`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:21:46 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 17:19:41 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Thu, 29 Jul 2021 00:23:24 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:23:24 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:23:24 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Thu, 29 Jul 2021 00:23:24 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:23:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:23:25 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c80b8bd2d83c8acb5fcaa6d64fec6f5d3d294d46f1567976afee5ba240a0d6`  
		Last Modified: Thu, 29 Jul 2021 00:25:33 GMT  
		Size: 747.9 KB (747867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d2714621edf634a2bfe5474f4a391445dde2a9fbc5252cd393f421f73ee755`  
		Last Modified: Thu, 29 Jul 2021 00:25:32 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0-openssl` - linux; arm variant v6

```console
$ docker pull eclipse-mosquitto@sha256:db52d87d2c4eb6386811d96f5dbe1a2c78e1f46df8a1d48fdf4b78c86dd0262f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3313989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:664e1b21126264b0b045dbc7cdbfe28f9af81f1b8b69386775738650dbaf615e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:51:14 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:51:14 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:53:36 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:53:36 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:53:37 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:53:37 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:53:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:53:38 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ccb38e36f37ca6646fb20a7cdb1b2a5b7e147064198abc051f661711d9800`  
		Last Modified: Wed, 28 Jul 2021 23:58:20 GMT  
		Size: 708.4 KB (708369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d77c03049a432ecb5029af93e3a92a230cce4513c13633d843f634a9ee68ea5`  
		Last Modified: Wed, 28 Jul 2021 23:58:20 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0-openssl` - linux; arm64 variant v8

```console
$ docker pull eclipse-mosquitto@sha256:56669361c3ce0cba5da58075d399f2a1f3dbc1d71d50f44715ce0c8fea96b746
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3454751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d487ad59fd2c73679cd52f9291c36625b26e440cc74a1a83b55dd5ea65cb7ff`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:33:08 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Tue, 15 Jun 2021 23:33:08 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:49:59 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:49:59 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:49:59 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:49:59 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:49:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:50:00 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75ec133029338b56c30de97bb847ca01bfb16aebc0ff5c576e9ab900a4364b8`  
		Last Modified: Wed, 28 Jul 2021 23:52:27 GMT  
		Size: 743.7 KB (743689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5e61cfd4deb3d00131ec56368c51781e579e550ead1242ba84dbbf868e5421`  
		Last Modified: Wed, 28 Jul 2021 23:52:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0-openssl` - linux; 386

```console
$ docker pull eclipse-mosquitto@sha256:78ebe2cbd2a1265f008c405041587c4d3063c5ab1dec755b876227002ef2dc1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3575739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6775b7c456948e0455209005da7c2c0d85a82807dc8fdd0b1530ee3b7234f7e2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:38:43 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 18:25:50 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:43:41 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:43:41 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:43:42 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:43:42 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:43:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:43:43 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d70dba08366c843b421aa6ed16675ea19159ec167a740b6d498ce618bd48972`  
		Last Modified: Wed, 28 Jul 2021 23:46:43 GMT  
		Size: 779.6 KB (779577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2b828537676a2beb7525de65a180944e17c9ecb16055fc2344957b95011c27`  
		Last Modified: Wed, 28 Jul 2021 23:46:43 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0-openssl` - linux; ppc64le

```console
$ docker pull eclipse-mosquitto@sha256:369cf5d4e988adff6b57b4d684109616abe6bdb1f99c5f93b497572d9fcc2213
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3627887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb9702fc0f39ed65d1e770bacf7b03009b0c6ac0dd6d11a15584bb0e1b49c0a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Thu, 29 Jul 2021 00:23:29 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Thu, 29 Jul 2021 00:23:37 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Thu, 29 Jul 2021 00:26:36 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:26:46 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:26:53 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Thu, 29 Jul 2021 00:27:05 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:27:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:27:24 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f894f1cd17c1894dd8edbf22593f163ca65075b8cc46dc10013bf5d5dc2991`  
		Last Modified: Thu, 29 Jul 2021 00:33:28 GMT  
		Size: 820.8 KB (820769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f6feee539bd2ca5bdeb92ca6757e5ce9faae07c52f9f05fc4a9661bedecd38`  
		Last Modified: Thu, 29 Jul 2021 00:33:27 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0-openssl` - linux; s390x

```console
$ docker pull eclipse-mosquitto@sha256:dec6a71c656ca265bfc82be5abb61a2d7e61c6eb621d394aef4c8355e677834c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3307538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:080b10312d76f275fa738e7f2b07479dd610fcb30632de1e62eeba77c059b6a0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:46:00 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:46:00 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:47:11 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:47:11 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:47:12 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:47:12 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:47:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:47:12 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081619879b747e9d716c5dcbb56fce0ea44dda274ccfcd25a63f6d639bcbe067`  
		Last Modified: Wed, 28 Jul 2021 23:49:27 GMT  
		Size: 738.7 KB (738742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03aa253a5b6b699f75c7a54a0205d8fd44fdff9b3d35c89e80789e6bb0af8432`  
		Last Modified: Wed, 28 Jul 2021 23:49:27 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eclipse-mosquitto:2.0.11`

```console
$ docker pull eclipse-mosquitto@sha256:8f80383b4c14b6fcfbfb23b7d6014b6c7fc7ef9c3f7d6ae8fd12d286d81acc46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-mosquitto:2.0.11` - linux; amd64

```console
$ docker pull eclipse-mosquitto@sha256:610eaf4aadce8090d4a6af580788189272ca9ba39671cd9ab02f47df9ed0461e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4733862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a8baae5c3fc5eb59fa173f9acc042c276fc204e371b834b7b32326f2197480`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:21:46 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 17:19:41 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Thu, 29 Jul 2021 00:22:34 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:22:34 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:22:34 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Thu, 29 Jul 2021 00:22:35 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:22:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:22:35 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c621ea1b2e689a87634043f08d91fe28277b1024847ba4d2ddac287c36e147`  
		Last Modified: Thu, 29 Jul 2021 00:25:18 GMT  
		Size: 1.9 MB (1932927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5a90f7f9abbe83f31858a296b8ac2347ae474d982c30c6c78a363432d16420`  
		Last Modified: Thu, 29 Jul 2021 00:25:17 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0.11` - linux; arm variant v6

```console
$ docker pull eclipse-mosquitto@sha256:efbb43243a562aa47fbba37e3d71be61d2ff78c035b84913324ca7a281cd23c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4376622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0118196891ad1173e90238ddc67e90cd805c5fb0333d37f52b6ed94119cb93bb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:51:14 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:51:14 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:52:17 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:52:18 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:52:19 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:52:19 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:52:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:52:20 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfa3e90898f09f982660e08d7d057e186d0da403ba25b059f991cdec11d1620`  
		Last Modified: Wed, 28 Jul 2021 23:58:00 GMT  
		Size: 1.8 MB (1771001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc49daa6fb8480af875b9239c9f282479d6c88ac6c613ed39d8c94110420779`  
		Last Modified: Wed, 28 Jul 2021 23:58:00 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0.11` - linux; arm64 variant v8

```console
$ docker pull eclipse-mosquitto@sha256:42e95a9a11914eba10106bb7d2b8be09d2416f20bf602a244615201c2d63b700
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4617441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cfb93cbd7e20c634f535c8b2ec3e67a51332a25a17f1de08cd8fe46e0cdcb85`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:33:08 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Tue, 15 Jun 2021 23:33:08 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:49:15 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:49:15 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:49:15 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:49:15 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:49:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:49:16 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf6e679922572c915d192412351500f438150c207acd6dae70a25c94a85dfb9`  
		Last Modified: Wed, 28 Jul 2021 23:52:09 GMT  
		Size: 1.9 MB (1906379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a310f4cbd62b3af8de7f3e77c7ecde0525b23ff5e07888b48e324f8c06aacf94`  
		Last Modified: Wed, 28 Jul 2021 23:52:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0.11` - linux; 386

```console
$ docker pull eclipse-mosquitto@sha256:3612394bbc5ac0d52f091bb368e821d89e691082bf16e3eb5ebcfaf557318016
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4847770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:083368fe7e4f2a2c24bcab9cfb488bae1ff09c107a34988515e65b6ada996e8b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:38:43 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 18:25:50 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:42:43 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:42:43 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:42:44 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:42:44 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:42:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:42:44 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51797827808a88c53d628823b4ecbd55c66d931e48c2262e4d2356c08f1052a`  
		Last Modified: Wed, 28 Jul 2021 23:46:25 GMT  
		Size: 2.1 MB (2051608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe73ed5d711a9a6f334bc5e0459bd82b9f86d04900dd2310348ec7813ee3707`  
		Last Modified: Wed, 28 Jul 2021 23:46:24 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0.11` - linux; ppc64le

```console
$ docker pull eclipse-mosquitto@sha256:a339579b235aaf7224551ba16f739c585e12e99c9a9dc40b4f1d5d39ce8b1dab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4846083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f83924be6138538b0f5fd17f69726095075c336aeb0fab2e0381d1a618d59bc4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Thu, 29 Jul 2021 00:23:29 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Thu, 29 Jul 2021 00:23:37 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Thu, 29 Jul 2021 00:24:45 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:24:56 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:24:59 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Thu, 29 Jul 2021 00:25:05 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:25:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:25:20 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4778c7030906a8e96907db2897a87a9674b97e78edaff18b1c934eece90ef4`  
		Last Modified: Thu, 29 Jul 2021 00:33:10 GMT  
		Size: 2.0 MB (2038966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674bebb6c7890560f8749875d7964eb35130983172bed3cbbd9335b86eb23f1a`  
		Last Modified: Thu, 29 Jul 2021 00:33:09 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0.11` - linux; s390x

```console
$ docker pull eclipse-mosquitto@sha256:d5a2274bf3061aeee30c0d48dc42bad0389919f1db755cb2b6143c7eaf8271e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4518101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f7a06b56186bb8148b90ffcd305cccab9102df332ecb1c29a425e52dd066e3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:46:00 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:46:00 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:46:33 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:46:33 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:46:33 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:46:34 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:46:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:46:34 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e5e08ac493722d7e19825df6caeab115dcec2dcb207fb5d7981c511163c5e4`  
		Last Modified: Wed, 28 Jul 2021 23:49:16 GMT  
		Size: 1.9 MB (1949305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c409893653081bff1b92986bf8bd505c059b445d8014c545a4e7bdb12ca006a1`  
		Last Modified: Wed, 28 Jul 2021 23:49:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eclipse-mosquitto:2.0.11-openssl`

```console
$ docker pull eclipse-mosquitto@sha256:3d83387a181d1a8e5a1f14bbb2b36d695d33acbcfed55c60fb6f75c4de5f13d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-mosquitto:2.0.11-openssl` - linux; amd64

```console
$ docker pull eclipse-mosquitto@sha256:de5c92f91918beb14133e1c5c2bc2f88096d28124e4b2f007c8d67cb9ad98df6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3548802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b658f2c808c9d64c61e43a04d3f7dc3fbc72da473f31e06b7838762a634c027`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:21:46 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 17:19:41 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Thu, 29 Jul 2021 00:23:24 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:23:24 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:23:24 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Thu, 29 Jul 2021 00:23:24 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:23:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:23:25 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c80b8bd2d83c8acb5fcaa6d64fec6f5d3d294d46f1567976afee5ba240a0d6`  
		Last Modified: Thu, 29 Jul 2021 00:25:33 GMT  
		Size: 747.9 KB (747867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d2714621edf634a2bfe5474f4a391445dde2a9fbc5252cd393f421f73ee755`  
		Last Modified: Thu, 29 Jul 2021 00:25:32 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0.11-openssl` - linux; arm variant v6

```console
$ docker pull eclipse-mosquitto@sha256:db52d87d2c4eb6386811d96f5dbe1a2c78e1f46df8a1d48fdf4b78c86dd0262f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3313989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:664e1b21126264b0b045dbc7cdbfe28f9af81f1b8b69386775738650dbaf615e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:51:14 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:51:14 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:53:36 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:53:36 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:53:37 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:53:37 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:53:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:53:38 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ccb38e36f37ca6646fb20a7cdb1b2a5b7e147064198abc051f661711d9800`  
		Last Modified: Wed, 28 Jul 2021 23:58:20 GMT  
		Size: 708.4 KB (708369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d77c03049a432ecb5029af93e3a92a230cce4513c13633d843f634a9ee68ea5`  
		Last Modified: Wed, 28 Jul 2021 23:58:20 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0.11-openssl` - linux; arm64 variant v8

```console
$ docker pull eclipse-mosquitto@sha256:56669361c3ce0cba5da58075d399f2a1f3dbc1d71d50f44715ce0c8fea96b746
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3454751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d487ad59fd2c73679cd52f9291c36625b26e440cc74a1a83b55dd5ea65cb7ff`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:33:08 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Tue, 15 Jun 2021 23:33:08 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:49:59 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:49:59 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:49:59 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:49:59 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:49:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:50:00 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75ec133029338b56c30de97bb847ca01bfb16aebc0ff5c576e9ab900a4364b8`  
		Last Modified: Wed, 28 Jul 2021 23:52:27 GMT  
		Size: 743.7 KB (743689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5e61cfd4deb3d00131ec56368c51781e579e550ead1242ba84dbbf868e5421`  
		Last Modified: Wed, 28 Jul 2021 23:52:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0.11-openssl` - linux; 386

```console
$ docker pull eclipse-mosquitto@sha256:78ebe2cbd2a1265f008c405041587c4d3063c5ab1dec755b876227002ef2dc1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3575739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6775b7c456948e0455209005da7c2c0d85a82807dc8fdd0b1530ee3b7234f7e2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:38:43 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 18:25:50 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:43:41 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:43:41 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:43:42 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:43:42 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:43:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:43:43 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d70dba08366c843b421aa6ed16675ea19159ec167a740b6d498ce618bd48972`  
		Last Modified: Wed, 28 Jul 2021 23:46:43 GMT  
		Size: 779.6 KB (779577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2b828537676a2beb7525de65a180944e17c9ecb16055fc2344957b95011c27`  
		Last Modified: Wed, 28 Jul 2021 23:46:43 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0.11-openssl` - linux; ppc64le

```console
$ docker pull eclipse-mosquitto@sha256:369cf5d4e988adff6b57b4d684109616abe6bdb1f99c5f93b497572d9fcc2213
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3627887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb9702fc0f39ed65d1e770bacf7b03009b0c6ac0dd6d11a15584bb0e1b49c0a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Thu, 29 Jul 2021 00:23:29 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Thu, 29 Jul 2021 00:23:37 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Thu, 29 Jul 2021 00:26:36 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:26:46 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:26:53 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Thu, 29 Jul 2021 00:27:05 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:27:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:27:24 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f894f1cd17c1894dd8edbf22593f163ca65075b8cc46dc10013bf5d5dc2991`  
		Last Modified: Thu, 29 Jul 2021 00:33:28 GMT  
		Size: 820.8 KB (820769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f6feee539bd2ca5bdeb92ca6757e5ce9faae07c52f9f05fc4a9661bedecd38`  
		Last Modified: Thu, 29 Jul 2021 00:33:27 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:2.0.11-openssl` - linux; s390x

```console
$ docker pull eclipse-mosquitto@sha256:dec6a71c656ca265bfc82be5abb61a2d7e61c6eb621d394aef4c8355e677834c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3307538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:080b10312d76f275fa738e7f2b07479dd610fcb30632de1e62eeba77c059b6a0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:46:00 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:46:00 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:47:11 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:47:11 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:47:12 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:47:12 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:47:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:47:12 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081619879b747e9d716c5dcbb56fce0ea44dda274ccfcd25a63f6d639bcbe067`  
		Last Modified: Wed, 28 Jul 2021 23:49:27 GMT  
		Size: 738.7 KB (738742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03aa253a5b6b699f75c7a54a0205d8fd44fdff9b3d35c89e80789e6bb0af8432`  
		Last Modified: Wed, 28 Jul 2021 23:49:27 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eclipse-mosquitto:latest`

```console
$ docker pull eclipse-mosquitto@sha256:8f80383b4c14b6fcfbfb23b7d6014b6c7fc7ef9c3f7d6ae8fd12d286d81acc46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-mosquitto:latest` - linux; amd64

```console
$ docker pull eclipse-mosquitto@sha256:610eaf4aadce8090d4a6af580788189272ca9ba39671cd9ab02f47df9ed0461e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4733862 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c3a8baae5c3fc5eb59fa173f9acc042c276fc204e371b834b7b32326f2197480`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:21:46 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 17:19:41 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Thu, 29 Jul 2021 00:22:34 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:22:34 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:22:34 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Thu, 29 Jul 2021 00:22:35 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:22:35 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:22:35 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32c621ea1b2e689a87634043f08d91fe28277b1024847ba4d2ddac287c36e147`  
		Last Modified: Thu, 29 Jul 2021 00:25:18 GMT  
		Size: 1.9 MB (1932927 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5b5a90f7f9abbe83f31858a296b8ac2347ae474d982c30c6c78a363432d16420`  
		Last Modified: Thu, 29 Jul 2021 00:25:17 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:latest` - linux; arm variant v6

```console
$ docker pull eclipse-mosquitto@sha256:efbb43243a562aa47fbba37e3d71be61d2ff78c035b84913324ca7a281cd23c5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.4 MB (4376622 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0118196891ad1173e90238ddc67e90cd805c5fb0333d37f52b6ed94119cb93bb`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:51:14 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:51:14 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:52:17 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:52:18 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:52:19 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:52:19 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:52:20 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:52:20 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ccfa3e90898f09f982660e08d7d057e186d0da403ba25b059f991cdec11d1620`  
		Last Modified: Wed, 28 Jul 2021 23:58:00 GMT  
		Size: 1.8 MB (1771001 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4bc49daa6fb8480af875b9239c9f282479d6c88ac6c613ed39d8c94110420779`  
		Last Modified: Wed, 28 Jul 2021 23:58:00 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:latest` - linux; arm64 variant v8

```console
$ docker pull eclipse-mosquitto@sha256:42e95a9a11914eba10106bb7d2b8be09d2416f20bf602a244615201c2d63b700
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.6 MB (4617441 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1cfb93cbd7e20c634f535c8b2ec3e67a51332a25a17f1de08cd8fe46e0cdcb85`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:33:08 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Tue, 15 Jun 2021 23:33:08 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:49:15 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:49:15 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:49:15 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:49:15 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:49:15 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:49:16 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5bf6e679922572c915d192412351500f438150c207acd6dae70a25c94a85dfb9`  
		Last Modified: Wed, 28 Jul 2021 23:52:09 GMT  
		Size: 1.9 MB (1906379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a310f4cbd62b3af8de7f3e77c7ecde0525b23ff5e07888b48e324f8c06aacf94`  
		Last Modified: Wed, 28 Jul 2021 23:52:08 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:latest` - linux; 386

```console
$ docker pull eclipse-mosquitto@sha256:3612394bbc5ac0d52f091bb368e821d89e691082bf16e3eb5ebcfaf557318016
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4847770 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:083368fe7e4f2a2c24bcab9cfb488bae1ff09c107a34988515e65b6ada996e8b`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:38:43 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 18:25:50 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:42:43 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:42:43 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:42:44 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:42:44 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:42:44 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:42:44 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c51797827808a88c53d628823b4ecbd55c66d931e48c2262e4d2356c08f1052a`  
		Last Modified: Wed, 28 Jul 2021 23:46:25 GMT  
		Size: 2.1 MB (2051608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ebe73ed5d711a9a6f334bc5e0459bd82b9f86d04900dd2310348ec7813ee3707`  
		Last Modified: Wed, 28 Jul 2021 23:46:24 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:latest` - linux; ppc64le

```console
$ docker pull eclipse-mosquitto@sha256:a339579b235aaf7224551ba16f739c585e12e99c9a9dc40b4f1d5d39ce8b1dab
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.8 MB (4846083 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f83924be6138538b0f5fd17f69726095075c336aeb0fab2e0381d1a618d59bc4`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Thu, 29 Jul 2021 00:23:29 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Thu, 29 Jul 2021 00:23:37 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Thu, 29 Jul 2021 00:24:45 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:24:56 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:24:59 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Thu, 29 Jul 2021 00:25:05 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:25:11 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:25:20 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0c4778c7030906a8e96907db2897a87a9674b97e78edaff18b1c934eece90ef4`  
		Last Modified: Thu, 29 Jul 2021 00:33:10 GMT  
		Size: 2.0 MB (2038966 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:674bebb6c7890560f8749875d7964eb35130983172bed3cbbd9335b86eb23f1a`  
		Last Modified: Thu, 29 Jul 2021 00:33:09 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:latest` - linux; s390x

```console
$ docker pull eclipse-mosquitto@sha256:d5a2274bf3061aeee30c0d48dc42bad0389919f1db755cb2b6143c7eaf8271e5
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4518101 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:33f7a06b56186bb8148b90ffcd305cccab9102df332ecb1c29a425e52dd066e3`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:46:00 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:46:00 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:46:33 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         libressl-dev         linux-headers         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_TLS_PSK=no         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates         libressl &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:46:33 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:46:33 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:46:34 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:46:34 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:46:34 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38e5e08ac493722d7e19825df6caeab115dcec2dcb207fb5d7981c511163c5e4`  
		Last Modified: Wed, 28 Jul 2021 23:49:16 GMT  
		Size: 1.9 MB (1949305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c409893653081bff1b92986bf8bd505c059b445d8014c545a4e7bdb12ca006a1`  
		Last Modified: Wed, 28 Jul 2021 23:49:15 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

## `eclipse-mosquitto:openssl`

```console
$ docker pull eclipse-mosquitto@sha256:3d83387a181d1a8e5a1f14bbb2b36d695d33acbcfed55c60fb6f75c4de5f13d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 6
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm64 variant v8
	-	linux; 386
	-	linux; ppc64le
	-	linux; s390x

### `eclipse-mosquitto:openssl` - linux; amd64

```console
$ docker pull eclipse-mosquitto@sha256:de5c92f91918beb14133e1c5c2bc2f88096d28124e4b2f007c8d67cb9ad98df6
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3548802 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6b658f2c808c9d64c61e43a04d3f7dc3fbc72da473f31e06b7838762a634c027`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:21:46 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 17:19:41 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Thu, 29 Jul 2021 00:23:24 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:23:24 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:23:24 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Thu, 29 Jul 2021 00:23:24 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:23:25 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:23:25 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:99c80b8bd2d83c8acb5fcaa6d64fec6f5d3d294d46f1567976afee5ba240a0d6`  
		Last Modified: Thu, 29 Jul 2021 00:25:33 GMT  
		Size: 747.9 KB (747867 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b8d2714621edf634a2bfe5474f4a391445dde2a9fbc5252cd393f421f73ee755`  
		Last Modified: Thu, 29 Jul 2021 00:25:32 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:openssl` - linux; arm variant v6

```console
$ docker pull eclipse-mosquitto@sha256:db52d87d2c4eb6386811d96f5dbe1a2c78e1f46df8a1d48fdf4b78c86dd0262f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3313989 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:664e1b21126264b0b045dbc7cdbfe28f9af81f1b8b69386775738650dbaf615e`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 22:57:41 GMT
ADD file:82fa6a18d24e3f535c9061d2e111d63fe6d8a27710bb34a17b326e605ff478be in / 
# Tue, 15 Jun 2021 22:57:41 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:51:14 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:51:14 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:53:36 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:53:36 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:53:37 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:53:37 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:53:38 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:53:38 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:b452d2916bdfd021add56f1eda6bdea35400671ef07b38316ef82fce92a88fee`  
		Last Modified: Wed, 14 Apr 2021 18:50:38 GMT  
		Size: 2.6 MB (2605253 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:534ccb38e36f37ca6646fb20a7cdb1b2a5b7e147064198abc051f661711d9800`  
		Last Modified: Wed, 28 Jul 2021 23:58:20 GMT  
		Size: 708.4 KB (708369 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d77c03049a432ecb5029af93e3a92a230cce4513c13633d843f634a9ee68ea5`  
		Last Modified: Wed, 28 Jul 2021 23:58:20 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:openssl` - linux; arm64 variant v8

```console
$ docker pull eclipse-mosquitto@sha256:56669361c3ce0cba5da58075d399f2a1f3dbc1d71d50f44715ce0c8fea96b746
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.5 MB (3454751 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9d487ad59fd2c73679cd52f9291c36625b26e440cc74a1a83b55dd5ea65cb7ff`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Tue, 15 Jun 2021 21:45:09 GMT
ADD file:3db1e10ac5ebf1cb34939eff736f1384f7d3b17355758cec361489fa7a7e19ca in / 
# Tue, 15 Jun 2021 21:45:09 GMT
CMD ["/bin/sh"]
# Tue, 15 Jun 2021 23:33:08 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Tue, 15 Jun 2021 23:33:08 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:49:59 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:49:59 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:49:59 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:49:59 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:49:59 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:50:00 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:d2f70382dc9a1658ea3491d7ab4439c22087e426c00e3eb7daf825b83be4ba9c`  
		Last Modified: Wed, 14 Apr 2021 18:43:55 GMT  
		Size: 2.7 MB (2710694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b75ec133029338b56c30de97bb847ca01bfb16aebc0ff5c576e9ab900a4364b8`  
		Last Modified: Wed, 28 Jul 2021 23:52:27 GMT  
		Size: 743.7 KB (743689 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e5e61cfd4deb3d00131ec56368c51781e579e550ead1242ba84dbbf868e5421`  
		Last Modified: Wed, 28 Jul 2021 23:52:26 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:openssl` - linux; 386

```console
$ docker pull eclipse-mosquitto@sha256:78ebe2cbd2a1265f008c405041587c4d3063c5ab1dec755b876227002ef2dc1f
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3575739 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6775b7c456948e0455209005da7c2c0d85a82807dc8fdd0b1530ee3b7234f7e2`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:38:36 GMT
ADD file:0a694887033953f24197dedcb1098d28a4b6e539b29386f53d82262107e208fb in / 
# Wed, 14 Apr 2021 18:38:36 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 23:38:43 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 09 Jun 2021 18:25:50 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:43:41 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:43:41 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:43:42 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:43:42 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:43:42 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:43:43 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:7aa04a8f7710c18952348aa54b4346438ad013c87b6f7d476eb21ad756359bc3`  
		Last Modified: Wed, 14 Apr 2021 18:39:43 GMT  
		Size: 2.8 MB (2795795 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d70dba08366c843b421aa6ed16675ea19159ec167a740b6d498ce618bd48972`  
		Last Modified: Wed, 28 Jul 2021 23:46:43 GMT  
		Size: 779.6 KB (779577 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6f2b828537676a2beb7525de65a180944e17c9ecb16055fc2344957b95011c27`  
		Last Modified: Wed, 28 Jul 2021 23:46:43 GMT  
		Size: 367.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:openssl` - linux; ppc64le

```console
$ docker pull eclipse-mosquitto@sha256:369cf5d4e988adff6b57b4d684109616abe6bdb1f99c5f93b497572d9fcc2213
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.6 MB (3627887 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bb9702fc0f39ed65d1e770bacf7b03009b0c6ac0dd6d11a15584bb0e1b49c0a`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 19:31:22 GMT
ADD file:f8b081207f6d35f8ebd06aa471e350644151d183801f678def586d8f37e81366 in / 
# Wed, 14 Apr 2021 19:31:29 GMT
CMD ["/bin/sh"]
# Thu, 29 Jul 2021 00:23:29 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Thu, 29 Jul 2021 00:23:37 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Thu, 29 Jul 2021 00:26:36 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Thu, 29 Jul 2021 00:26:46 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Thu, 29 Jul 2021 00:26:53 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Thu, 29 Jul 2021 00:27:05 GMT
EXPOSE 1883
# Thu, 29 Jul 2021 00:27:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Thu, 29 Jul 2021 00:27:24 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:45707b9629c4ab8c6046680737229218fe844f38d08e5458b24605e1dbfd2709`  
		Last Modified: Wed, 14 Apr 2021 19:32:50 GMT  
		Size: 2.8 MB (2806750 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:34f894f1cd17c1894dd8edbf22593f163ca65075b8cc46dc10013bf5d5dc2991`  
		Last Modified: Thu, 29 Jul 2021 00:33:28 GMT  
		Size: 820.8 KB (820769 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:31f6feee539bd2ca5bdeb92ca6757e5ce9faae07c52f9f05fc4a9661bedecd38`  
		Last Modified: Thu, 29 Jul 2021 00:33:27 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `eclipse-mosquitto:openssl` - linux; s390x

```console
$ docker pull eclipse-mosquitto@sha256:dec6a71c656ca265bfc82be5abb61a2d7e61c6eb621d394aef4c8355e677834c
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **3.3 MB (3307538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:080b10312d76f275fa738e7f2b07479dd610fcb30632de1e62eeba77c059b6a0`
-	Entrypoint: `["\/docker-entrypoint.sh"]`
-	Default Command: `["\/usr\/sbin\/mosquitto","-c","\/mosquitto\/config\/mosquitto.conf"]`

```dockerfile
# Wed, 14 Apr 2021 18:41:42 GMT
ADD file:c73a5ff435939cdc9d621ee9dc2aa5a54a5f5e0241caae8dc948c03c423d9fef in / 
# Wed, 14 Apr 2021 18:41:42 GMT
CMD ["/bin/sh"]
# Wed, 28 Jul 2021 23:46:00 GMT
LABEL maintainer=Roger Light <roger@atchoo.org> description=Eclipse Mosquitto MQTT Broker
# Wed, 28 Jul 2021 23:46:00 GMT
ENV VERSION=2.0.11 DOWNLOAD_SHA256=7b36a7198bce85cf31b132f5c6ee36dcf5dadf86fb768501eb1e11ce95d4f78a GPG_KEYS=A0D6EEA1DCAE49A635A3B2F0779B22DFB3E717B7 LWS_VERSION=4.2.0 LWS_SHA256=a57e9a4765dbcd4d880feba8089b43ed69995eaf10d5d61a07981d9ddd975f40 CJSON_VERSION=1.7.14 CJSON_SHA256=fb50a663eefdc76bafa80c82bc045af13b1363e8f45cec8b442007aef6a41343
# Wed, 28 Jul 2021 23:47:11 GMT
RUN set -x &&     apk --no-cache add --virtual build-deps         build-base         cmake         gnupg         linux-headers         openssl-dev         util-linux-dev &&     wget https://github.com/warmcat/libwebsockets/archive/v${LWS_VERSION}.tar.gz -O /tmp/lws.tar.gz &&     echo "$LWS_SHA256  /tmp/lws.tar.gz" | sha256sum -c - &&     mkdir -p /build/lws &&     tar --strip=1 -xf /tmp/lws.tar.gz -C /build/lws &&     rm /tmp/lws.tar.gz &&     cd /build/lws &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DCMAKE_INSTALL_PREFIX=/usr         -DDISABLE_WERROR=ON         -DLWS_IPV6=ON         -DLWS_WITHOUT_BUILTIN_GETIFADDRS=ON         -DLWS_WITHOUT_CLIENT=ON         -DLWS_WITHOUT_EXTENSIONS=ON         -DLWS_WITHOUT_TESTAPPS=ON         -DLWS_WITH_EXTERNAL_POLL=ON         -DLWS_WITH_HTTP2=OFF         -DLWS_WITH_SHARED=OFF         -DLWS_WITH_ZIP_FOPS=OFF         -DLWS_WITH_ZLIB=OFF &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://github.com/DaveGamble/cJSON/archive/v${CJSON_VERSION}.tar.gz -O /tmp/cjson.tar.gz &&     echo "$CJSON_SHA256  /tmp/cjson.tar.gz" | sha256sum -c - &&     mkdir -p /build/cjson &&     tar --strip=1 -xf /tmp/cjson.tar.gz -C /build/cjson &&     rm /tmp/cjson.tar.gz &&     cd /build/cjson &&     cmake .         -DCMAKE_BUILD_TYPE=MinSizeRel         -DBUILD_SHARED_AND_STATIC_LIBS=OFF         -DBUILD_SHARED_LIBS=OFF         -DCJSON_BUILD_SHARED_LIBS=OFF         -DCJSON_OVERRIDE_BUILD_SHARED_LIBS=OFF         -DCMAKE_INSTALL_PREFIX=/usr &&     make -j "$(nproc)" &&     rm -rf /root/.cmake &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz -O /tmp/mosq.tar.gz &&     echo "$DOWNLOAD_SHA256  /tmp/mosq.tar.gz" | sha256sum -c - &&     wget https://mosquitto.org/files/source/mosquitto-${VERSION}.tar.gz.asc -O /tmp/mosq.tar.gz.asc &&     export GNUPGHOME="$(mktemp -d)" &&     found='';     for server in         ha.pool.sks-keyservers.net         hkp://keyserver.ubuntu.com:80         hkp://p80.pool.sks-keyservers.net:80         pgp.mit.edu     ; do         echo "Fetching GPG key $GPG_KEYS from $server";         gpg --keyserver "$server" --keyserver-options timeout=10 --recv-keys "$GPG_KEYS" && found=yes && break;     done;     test -z "$found" && echo >&2 "error: failed to fetch GPG key $GPG_KEYS" && exit 1;     gpg --batch --verify /tmp/mosq.tar.gz.asc /tmp/mosq.tar.gz &&     gpgconf --kill all &&     rm -rf "$GNUPGHOME" /tmp/mosq.tar.gz.asc &&     mkdir -p /build/mosq &&     tar --strip=1 -xf /tmp/mosq.tar.gz -C /build/mosq &&     rm /tmp/mosq.tar.gz &&     make -C /build/mosq -j "$(nproc)"         CFLAGS="-Wall -O2 -I/build/lws/include -I/build"         LDFLAGS="-L/build/lws/lib -L/build/cjson"         WITH_ADNS=no         WITH_DOCS=no         WITH_SHARED_LIBRARIES=yes         WITH_SRV=no         WITH_STRIP=yes         WITH_WEBSOCKETS=yes         prefix=/usr         binary &&     addgroup -S -g 1883 mosquitto 2>/dev/null &&     adduser -S -u 1883 -D -H -h /var/empty -s /sbin/nologin -G mosquitto -g mosquitto mosquitto 2>/dev/null &&     mkdir -p /mosquitto/config /mosquitto/data /mosquitto/log &&     install -d /usr/sbin/ &&     install -s -m755 /build/mosq/client/mosquitto_pub /usr/bin/mosquitto_pub &&     install -s -m755 /build/mosq/client/mosquitto_rr /usr/bin/mosquitto_rr &&     install -s -m755 /build/mosq/client/mosquitto_sub /usr/bin/mosquitto_sub &&     install -s -m644 /build/mosq/lib/libmosquitto.so.1 /usr/lib/libmosquitto.so.1 &&     install -s -m755 /build/mosq/src/mosquitto /usr/sbin/mosquitto &&     install -s -m755 /build/mosq/apps/mosquitto_ctrl/mosquitto_ctrl /usr/bin/mosquitto_ctrl &&     install -s -m755 /build/mosq/apps/mosquitto_passwd/mosquitto_passwd /usr/bin/mosquitto_passwd &&     install -s -m755 /build/mosq/plugins/dynamic-security/mosquitto_dynamic_security.so /usr/lib/mosquitto_dynamic_security.so &&     install -m644 /build/mosq/mosquitto.conf /mosquitto/config/mosquitto.conf &&     install -Dm644 /build/cjson/LICENSE /usr/share/licenses/cJSON/LICENSE &&     install -Dm644 /build/lws/LICENSE /usr/share/licenses/libwebsockets/LICENSE &&     install -Dm644 /build/mosq/epl-v20 /usr/share/licenses/mosquitto/epl-v20 &&     install -Dm644 /build/mosq/edl-v10 /usr/share/licenses/mosquitto/edl-v10 &&     chown -R mosquitto:mosquitto /mosquitto &&     apk --no-cache add         ca-certificates &&     apk del build-deps &&     rm -rf /build
# Wed, 28 Jul 2021 23:47:11 GMT
VOLUME [/mosquitto/data /mosquitto/log]
# Wed, 28 Jul 2021 23:47:12 GMT
COPY multi:f828fb0704e6f46a450b717895e8dada966524fb8a3bd947f3ac0bd7ae28f571 in / 
# Wed, 28 Jul 2021 23:47:12 GMT
EXPOSE 1883
# Wed, 28 Jul 2021 23:47:12 GMT
ENTRYPOINT ["/docker-entrypoint.sh"]
# Wed, 28 Jul 2021 23:47:12 GMT
CMD ["/usr/sbin/mosquitto" "-c" "/mosquitto/config/mosquitto.conf"]
```

-	Layers:
	-	`sha256:27efec644c4207cbc4d1400f84f3402937aab5ce72489976148896e42a219820`  
		Last Modified: Wed, 14 Apr 2021 18:42:24 GMT  
		Size: 2.6 MB (2568428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:081619879b747e9d716c5dcbb56fce0ea44dda274ccfcd25a63f6d639bcbe067`  
		Last Modified: Wed, 28 Jul 2021 23:49:27 GMT  
		Size: 738.7 KB (738742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03aa253a5b6b699f75c7a54a0205d8fd44fdff9b3d35c89e80789e6bb0af8432`  
		Last Modified: Wed, 28 Jul 2021 23:49:27 GMT  
		Size: 368.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
