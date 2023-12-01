## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:112eaad8a7431b370c20d3adabe4b7ac4b0b9b2f83cabcf27ae54a104bf17d59
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	linux; amd64
	-	linux; arm64 variant v8

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:1193eee9874b2bce9065541569f5373d79243995f6ea9bce34056ce0425a6f6a
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **63.0 MB (62960873 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0bc4c6719bb3da7a75962469d87f12e5baf9f2ef5fda48fc2b05fd1d34ed878f`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 30 Nov 2023 23:22:52 GMT
ADD file:fc714080c3bcbbce7ac746a10d7b4355ffa36293a8d435d62cd5359ea8eb8364 in / 
# Thu, 30 Nov 2023 23:22:52 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 05:23:13 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 06:01:08 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 01 Dec 2023 06:01:21 GMT
ENV TELEGRAF_VERSION=1.28.5
# Fri, 01 Dec 2023 06:01:28 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 01 Dec 2023 06:01:28 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Dec 2023 06:01:28 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 01 Dec 2023 06:01:28 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 06:01:28 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:c926b61bad3b94ae7351bafd0c184c159ebf0643b085f7ef1d47ecdc7316833c`  
		Last Modified: Thu, 30 Nov 2023 23:23:28 GMT  
		Size: 3.4 MB (3402422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:703e958f39c4082f015dd7de32b1c116ef56e1e54010a31e991ec0c10e7feecc`  
		Last Modified: Fri, 01 Dec 2023 05:25:29 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:93f9134978c64af53ac70d7b738a210c1328d24dc1a25eb4d44d7173087a7a2f`  
		Last Modified: Fri, 01 Dec 2023 06:02:01 GMT  
		Size: 2.6 MB (2644946 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bbd66689949bc0bfbc2d37396f13a4ca79202368d001d9d9919c1a2e5cb214ec`  
		Last Modified: Fri, 01 Dec 2023 06:02:30 GMT  
		Size: 56.9 MB (56912898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a76b249b718bd8c689938b30cb54a35bd16c1559b0ec953bfbae3418c42dfcc1`  
		Last Modified: Fri, 01 Dec 2023 06:02:19 GMT  
		Size: 329.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `telegraf:alpine` - linux; arm64 variant v8

```console
$ docker pull telegraf@sha256:9abd92c798e7a04f30103b1c909296a6f752b93258711d6736f41565a14e77f6
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **57.6 MB (57594128 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b7c1be5420f2256037606879501b68b596b7270f939e5b0742cc880ce4da97cf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Thu, 30 Nov 2023 23:11:03 GMT
ADD file:d8a30995bbcd627f084912c728fda5483b6ba486de25af588a0956069d0bd7ad in / 
# Thu, 30 Nov 2023 23:11:03 GMT
CMD ["/bin/sh"]
# Fri, 01 Dec 2023 02:38:30 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Fri, 01 Dec 2023 09:29:37 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Fri, 01 Dec 2023 09:29:51 GMT
ENV TELEGRAF_VERSION=1.28.5
# Fri, 01 Dec 2023 09:29:56 GMT
RUN ARCH= &&     case "$(apk --print-arch)" in         x86_64) ARCH='amd64';;         aarch64) ARCH='arm64';;         *) echo "Unsupported architecture: $(apk --print-arch)"; exit 1;;     esac &&     set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz.asc telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_linux_${ARCH}.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Fri, 01 Dec 2023 09:29:57 GMT
EXPOSE 8092/udp 8094 8125/udp
# Fri, 01 Dec 2023 09:29:58 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Fri, 01 Dec 2023 09:29:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Fri, 01 Dec 2023 09:29:58 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:2c03dbb20264f09924f9eab176da44e5421e74a78b09531d3c63448a7baa7c59`  
		Last Modified: Thu, 30 Nov 2023 23:11:32 GMT  
		Size: 3.3 MB (3333033 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00f6ef2d119bdc2b844474b1941025c80c2a28072d415011a971ae3decceb4b8`  
		Last Modified: Fri, 01 Dec 2023 02:38:57 GMT  
		Size: 279.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7ca0a892394cd6b625d7d9cdb3d4bc69df64526779bd31ca9403a55bbbcca5c0`  
		Last Modified: Fri, 01 Dec 2023 09:30:27 GMT  
		Size: 2.7 MB (2673204 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a0966c76ccd38be27a8bf79cd4f6906012dfd128984fa170f86fea2cd6155461`  
		Last Modified: Fri, 01 Dec 2023 09:30:47 GMT  
		Size: 51.6 MB (51587284 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8d86eebfd2c91e08ee20d44fef32c1ac56d89958f0c0ec81ddd495f2c2011698`  
		Last Modified: Fri, 01 Dec 2023 09:30:41 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
