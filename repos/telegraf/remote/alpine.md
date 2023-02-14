## `telegraf:alpine`

```console
$ docker pull telegraf@sha256:5f8e4e68c928527997013b450849c4080d3f3fdde8fceccf995769d8b3b3f06c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `telegraf:alpine` - linux; amd64

```console
$ docker pull telegraf@sha256:4aa69cce85d7d9f6eb478a2a913aa3fb7ae4e69139a853a4e320d58440cf36e4
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **52.5 MB (52477643 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9649518e44c1b172c648867e3aa895eaad584f7ed4f64f512c6abad8dd6464d2`
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
# Tue, 14 Feb 2023 00:20:27 GMT
ENV TELEGRAF_VERSION=1.25.2
# Tue, 14 Feb 2023 00:20:33 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/telegraf/releases/telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     gpg --batch --verify telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz.asc telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mkdir -p /usr/src /etc/telegraf &&     tar -C /usr/src -xzf telegraf-${TELEGRAF_VERSION}_static_linux_amd64.tar.gz &&     mv /usr/src/telegraf*/etc/telegraf/telegraf.conf /etc/telegraf/ &&     mkdir /etc/telegraf/telegraf.d &&     cp -a /usr/src/telegraf*/usr/bin/telegraf /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps &&     addgroup -S telegraf &&     adduser -S telegraf -G telegraf &&     chown -R telegraf:telegraf /etc/telegraf
# Tue, 14 Feb 2023 00:20:33 GMT
EXPOSE 8092/udp 8094 8125/udp
# Tue, 14 Feb 2023 00:20:34 GMT
COPY file:f41cb64129e03c46523c3acd2da77376a68d9785d775faf0d359051c20b4f1bf in /entrypoint.sh 
# Tue, 14 Feb 2023 00:20:34 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Tue, 14 Feb 2023 00:20:34 GMT
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
	-	`sha256:fb3c31b28da4569a5041683f5798e26109236281de69401d20d1dfb49459e89a`  
		Last Modified: Tue, 14 Feb 2023 00:21:21 GMT  
		Size: 46.4 MB (46370997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92235faf2fe9f66b7cd08fe4db4357c829e05a80ae8fbf1d07142a94d73f4c3f`  
		Last Modified: Tue, 14 Feb 2023 00:21:14 GMT  
		Size: 326.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
