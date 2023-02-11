## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:bea089c3de38380f25f91734b3316bc5a91e5ae19eb54f6e5ae1b458ab6a6812
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:85b6283ead2a3fbb26c92ae2714109ee5a9f8f585260e3db4303866fc418f1bd
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.3 MB (52335060 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aefda4c867e477e2430048f1b3d6cc7ff647b4da60bdce35f445be71f392c857`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["telegraf"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:50 GMT
ADD file:ac5fb7eb0d68040d948989f0a50914d0d4a6b631cfe76b508eecd82eb7d46953 in / 
# Sat, 11 Feb 2023 04:46:50 GMT
CMD ["/bin/sh"]
# Sat, 11 Feb 2023 09:58:02 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Sat, 11 Feb 2023 14:07:54 GMT
RUN apk add --no-cache iputils ca-certificates net-snmp-tools procps lm_sensors tzdata su-exec libcap &&     update-ca-certificates
# Sat, 11 Feb 2023 14:08:22 GMT
ENV TELEGRAF_VERSION=1.25.1
# Sat, 11 Feb 2023 14:08:30 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Sat, 11 Feb 2023 14:08:31 GMT
EXPOSE 8092/udp 8094 8125/udp
# Sat, 11 Feb 2023 14:08:31 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Sat, 11 Feb 2023 14:08:31 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Sat, 11 Feb 2023 14:08:31 GMT
CMD ["telegraf"]
```

-	Layers:
	-	`sha256:ef5531b6e74e7865f5d142926b572d742ad47c153211de707903b4f5dd8d9e77`  
		Last Modified: Sat, 11 Feb 2023 04:47:32 GMT  
		Size: 2.8 MB (2807762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:78609e30990ccbdf3bf8ff0fb97d9cc3f1a128207e6de80aae40ce96e63cd92c`  
		Last Modified: Sat, 11 Feb 2023 14:08:49 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:23fe5f60e0243cd70ce085e0773498f72d2e22f37d66e8d91308d81e17f4e844`  
		Last Modified: Sat, 11 Feb 2023 14:08:50 GMT  
		Size: 3.3 MB (3298280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2f5114784c6e65a369eb5a9761a2ce77706e08b4830966f74063610b06377d1e`  
		Last Modified: Sat, 11 Feb 2023 14:09:29 GMT  
		Size: 46.2 MB (46228412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6368e6a47b774a80289888a06e3fbc07c7ae7e5be53edb90bb25ce3f3376e865`  
		Last Modified: Sat, 11 Feb 2023 14:09:21 GMT  
		Size: 328.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
