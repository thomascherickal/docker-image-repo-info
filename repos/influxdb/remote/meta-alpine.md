## `influxdb:meta-alpine`

```console
$ docker pull influxdb@sha256:50f6415fbcb9090b6f0137c3cc38c44958e3d817243fbb5d1c1fc47ad1ba0582
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:meta-alpine` - linux; amd64

```console
$ docker pull influxdb@sha256:f205bb2774db90735f516a996e01b953c85782db1d1f2c219a1747254ba29b08
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **27.0 MB (26967499 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:983e17d469ce4282fb747e4ed26a58357a467dfeff0b983e57864d550b93532a`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 14 Apr 2021 19:19:49 GMT
ADD file:4f526aa99067d82b341f7ca538f7826b7c23a628f1b615eea2883a2d434c1b90 in / 
# Wed, 14 Apr 2021 19:19:49 GMT
CMD ["/bin/sh"]
# Wed, 14 Apr 2021 20:12:38 GMT
RUN echo 'hosts: files dns' >> /etc/nsswitch.conf
# Wed, 14 Apr 2021 22:56:19 GMT
RUN apk add --no-cache tzdata bash ca-certificates &&     update-ca-certificates
# Wed, 14 Apr 2021 22:57:17 GMT
ENV INFLUXDB_VERSION=1.8.3-c1.8.3
# Wed, 14 Apr 2021 22:57:37 GMT
RUN set -ex &&     apk add --no-cache --virtual .build-deps wget gnupg tar &&     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     gpg --batch --verify influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz.asc influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     mkdir -p /usr/src &&     tar -C /usr/src -xzf influxdb-meta-${INFLUXDB_VERSION}-static_linux_amd64.tar.gz &&     rm -f /usr/src/influxdb-*/influxdb-meta.conf &&     chmod +x /usr/src/influxdb-*/* &&     cp -a /usr/src/influxdb-*/* /usr/bin/ &&     rm -rf *.tar.gz* /usr/src /root/.gnupg &&     apk del .build-deps
# Wed, 14 Apr 2021 22:57:38 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 14 Apr 2021 22:57:38 GMT
EXPOSE 8091
# Wed, 14 Apr 2021 22:57:38 GMT
VOLUME [/var/lib/influxdb]
# Wed, 14 Apr 2021 22:57:38 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 14 Apr 2021 22:57:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 14 Apr 2021 22:57:39 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:339de151aab4bc06eed8409daae147c408478cb538dacb90cc63f19ad4eba80b`  
		Last Modified: Wed, 14 Apr 2021 19:20:51 GMT  
		Size: 2.8 MB (2800567 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d4496f95da0ff203c55ba4ff45e6cc518bfd24507a21516931244d25e8db7d14`  
		Last Modified: Wed, 14 Apr 2021 20:13:37 GMT  
		Size: 154.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e1699ff2fb9d4dfb68fba8d9ca2ddea7f21d9a1e0b3e92a61555bec3b1f2369`  
		Last Modified: Wed, 14 Apr 2021 22:58:41 GMT  
		Size: 1.4 MB (1430783 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6842848fd72dae543e9cec2ee9a02273eb56bccb98e1df7a67ec462226702ff5`  
		Last Modified: Wed, 14 Apr 2021 23:00:39 GMT  
		Size: 22.7 MB (22735398 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b85af523caa3353e737b367b7ccf17b422372bf45cfcb707599dde1ef0ff30c0`  
		Last Modified: Wed, 14 Apr 2021 23:00:35 GMT  
		Size: 223.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4ff836b13b8350c6a99c8831862153092f5247e2e274d72ef884bbd98a46263c`  
		Last Modified: Wed, 14 Apr 2021 23:00:35 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
