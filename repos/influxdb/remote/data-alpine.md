## `influxdb:data-alpine`

```console
$ docker pull influxdb@sha256:261d1655b8cc2dc5404af459329701d0b8245717caadd711036a2e2a36888e36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:4062b21acf2700f04d0da13c37ecf473b0a75ac6de7b03c3f7fd4c3df2ce7524
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **61.4 MB (61352861 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:0f18f1dce311ade7a5bc787e5cc41b48cb635fb2e249b34189c63fbc882712b7`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Sat, 11 Feb 2023 04:46:42 GMT
ADD file:40887ab7c06977737e63c215c9bd297c0c74de8d12d16ebdf1c3d40ac392f62d in / 
# Sat, 11 Feb 2023 04:46:42 GMT
CMD ["/bin/sh"]
# Mon, 13 Mar 2023 23:20:24 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Mar 2023 00:54:52 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Thu, 16 Mar 2023 00:55:13 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 16 Mar 2023 00:55:21 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     gpgconf --kill all &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Thu, 16 Mar 2023 00:55:21 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 16 Mar 2023 00:55:21 GMT
EXPOSE 8086
# Thu, 16 Mar 2023 00:55:22 GMT
VOLUME [/var/lib/influxdb]
# Thu, 16 Mar 2023 00:55:22 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 16 Mar 2023 00:55:22 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 16 Mar 2023 00:55:22 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 16 Mar 2023 00:55:22 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:63b65145d645c1250c391b2d16ebe53b3747c295ca8ba2fcb6b0cf064a4dc21c`  
		Last Modified: Fri, 10 Feb 2023 22:41:31 GMT  
		Size: 3.4 MB (3374446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:69b7a2cbfc2f3b3305293d689573f3c9651d6053e5f780a9ba42a4c836d8d6c9`  
		Last Modified: Mon, 13 Mar 2023 23:21:18 GMT  
		Size: 278.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d5b0a9605b8bc1c4f3b877c51f73e8d0cc4b02403f8f9d18c276f012b604c038`  
		Last Modified: Thu, 16 Mar 2023 00:59:03 GMT  
		Size: 1.5 MB (1472712 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:61bad459754475dfd8621019d72d1bd32ca2b9be86fb936ab64308888ee0073a`  
		Last Modified: Thu, 16 Mar 2023 00:59:43 GMT  
		Size: 56.5 MB (56503629 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0fdd4464dd3872545334e618c0323eef93811cc622aa2409dc50a984d042034`  
		Last Modified: Thu, 16 Mar 2023 00:59:36 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aeb71d6736a13e612d2dc8a667133647ee9099895936ffa258569114cc772086`  
		Last Modified: Thu, 16 Mar 2023 00:59:36 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a34548e01d2f855e58fb7674a9102ca3878dda447d78e6060033d7827d27589f`  
		Last Modified: Thu, 16 Mar 2023 00:59:36 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
