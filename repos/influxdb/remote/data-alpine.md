## `influxdb:data-alpine`

```console
$ docker pull influxdb@sha256:fe6ac4f357e16b19ff202f3bb26c46b2705b294984e1675f46bce753d0694ea4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:b32206b0b89cd0b2366eed0298b2f983de3f64862bb38611b4b745b7b3353364
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **60.8 MB (60784165 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7f3952479650ac95cd5661233633ca18ec9d5b6c6b4aa43b5a254c367b3249d`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Fri, 27 Aug 2021 17:19:45 GMT
ADD file:aad4290d27580cc1a094ffaf98c3ca2fc5d699fe695dfb8e6e9fac20f1129450 in / 
# Fri, 27 Aug 2021 17:19:45 GMT
CMD ["/bin/sh"]
# Thu, 16 Sep 2021 21:20:06 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Thu, 16 Sep 2021 21:20:08 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Mon, 11 Oct 2021 23:20:37 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Mon, 11 Oct 2021 23:20:54 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-data-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Mon, 11 Oct 2021 23:20:54 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Mon, 11 Oct 2021 23:20:54 GMT
EXPOSE 8086
# Mon, 11 Oct 2021 23:20:54 GMT
VOLUME [/var/lib/influxdb]
# Mon, 11 Oct 2021 23:20:55 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Mon, 11 Oct 2021 23:20:55 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Mon, 11 Oct 2021 23:20:55 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Mon, 11 Oct 2021 23:20:55 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:a0d0a0d46f8b52473982a3c466318f479767577551a53ffc9074c9fa7035982e`  
		Last Modified: Fri, 27 Aug 2021 17:20:13 GMT  
		Size: 2.8 MB (2814446 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e8cf55ffd68f3512245522356168367182cfdaeb0a0d11bbd5328472d4c0761`  
		Last Modified: Thu, 16 Sep 2021 21:24:04 GMT  
		Size: 153.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7457db31b732bcfa93e8a40c987909364acc021b8a962de6d8f77e9a46830fee`  
		Last Modified: Thu, 16 Sep 2021 21:24:02 GMT  
		Size: 1.5 MB (1464176 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f617e688de2fe3e018e8342b0aef6fcb79cd667150730c3fe56cdca40f85c1af`  
		Last Modified: Mon, 11 Oct 2021 23:23:22 GMT  
		Size: 56.5 MB (56503592 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ba4436b7c1c928d1ac0f25d7e757e21f63fa25ee52e086579e3c3c61f674235f`  
		Last Modified: Mon, 11 Oct 2021 23:23:15 GMT  
		Size: 265.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5305554dc9907f47dfe620e9ab5934f66e7476ecd500796b0c115e80eb000849`  
		Last Modified: Mon, 11 Oct 2021 23:23:15 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9fc73aba05114206260f522c1fdfb34b05cdfa143b14829401f2d2ab1daa7728`  
		Last Modified: Mon, 11 Oct 2021 23:23:15 GMT  
		Size: 1.3 KB (1282 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
