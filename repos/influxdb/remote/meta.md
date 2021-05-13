## `influxdb:meta`

```console
$ docker pull influxdb@sha256:68fa2195ff557ce6c37d675589fe48dbc43b6cd90b20ac0078ad72aa7a333377
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:dc05a4e2cc33fbd9fe229abeea0771fb6df927cf487d360c7ca27e9c2266cd85
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **84.2 MB (84220023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d078f2f75f20c995dcdd5ab2bd6c9bc9d02df3ca79ab2df00e11847b9bb4a8bf`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Wed, 12 May 2021 01:23:05 GMT
ADD file:d9e4f6f4fc33703b766642a5642cabb2b01675bb55cf6050f2e91507577ff570 in / 
# Wed, 12 May 2021 01:23:06 GMT
CMD ["bash"]
# Wed, 12 May 2021 01:59:35 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		apt-transport-https 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 12 May 2021 01:59:42 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 12 May 2021 20:08:57 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver ha.pool.sks-keyservers.net --recv-keys "$key" ||         gpg --keyserver pgp.mit.edu --recv-keys "$key" ||         gpg --keyserver keyserver.pgp.com --recv-keys "$key" ;     done
# Wed, 12 May 2021 20:09:51 GMT
ENV INFLUXDB_VERSION=1.8.5-c1.8.5
# Wed, 12 May 2021 20:10:08 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 12 May 2021 20:10:08 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 12 May 2021 20:10:08 GMT
EXPOSE 8091
# Wed, 12 May 2021 20:10:08 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 May 2021 20:10:09 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 12 May 2021 20:10:09 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 May 2021 20:10:09 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:bfde2ec33fbca3c74c6e91bca3fbcb22ed2972671d49a1accb7089c9473cac12`  
		Last Modified: Wed, 12 May 2021 01:29:52 GMT  
		Size: 45.4 MB (45380083 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:787f5e2f10471c11a2064774062aeeb400f76e9eef1ca768156a23678f005f3e`  
		Last Modified: Wed, 12 May 2021 02:07:25 GMT  
		Size: 11.3 MB (11286410 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7b6173a10eb81a318ed53df74c8b80d29656f68194682e51f46f9b7b24c6ba03`  
		Last Modified: Wed, 12 May 2021 02:07:24 GMT  
		Size: 4.3 MB (4342456 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e7ee65a07cb0cad7eedb6332aad83a593a46bbae0a453842817353e2cf9de28d`  
		Last Modified: Wed, 12 May 2021 20:11:14 GMT  
		Size: 2.9 KB (2854 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b5c3aa7b43864264776e0705af60c7b648c6f35423a51c97aba06d9042b0fec6`  
		Last Modified: Wed, 12 May 2021 20:13:04 GMT  
		Size: 23.2 MB (23207651 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd009237bc2a719041f691f8a836e65ef361aafd7b4ce32e5561a79bf326c3c4`  
		Last Modified: Wed, 12 May 2021 20:13:00 GMT  
		Size: 196.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3a97dfb1738dd6efa509ec087257bcbe11511b70b7c2fe00c4b72df946dc2b19`  
		Last Modified: Wed, 12 May 2021 20:13:00 GMT  
		Size: 373.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
