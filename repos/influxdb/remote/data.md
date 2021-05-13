## `influxdb:data`

```console
$ docker pull influxdb@sha256:de7e74d5f1b459c92178fa5cb6462dc699566f3b4c12b28e46c1b6630b5cd8b1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:e21827a90a9bb76505e21d119f84ec4b449b251c24bab1ab15ecd8d26b85342b
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.8 MB (127762573 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:595c071ccfd76a0c907e702341b3392ba99a312f14d0abb2d3f8dd69a4ceda8b`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

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
# Wed, 12 May 2021 20:09:56 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 12 May 2021 20:09:57 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Wed, 12 May 2021 20:09:57 GMT
EXPOSE 8086
# Wed, 12 May 2021 20:09:57 GMT
VOLUME [/var/lib/influxdb]
# Wed, 12 May 2021 20:09:57 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Wed, 12 May 2021 20:09:58 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Wed, 12 May 2021 20:09:58 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 12 May 2021 20:09:58 GMT
CMD ["influxd"]
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
	-	`sha256:3f6fadffb19104f4088a82876015b9a09dcb684adee0b7d80ea2ac182d412dfa`  
		Last Modified: Wed, 12 May 2021 20:12:45 GMT  
		Size: 66.7 MB (66748997 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d6547be9217cc26fef15453ce9866313ee295825276eb53d3aa396dc63c5ea25`  
		Last Modified: Wed, 12 May 2021 20:12:36 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:171a5df9c7d640367018d467ec1ebf3d0c92632d2bb8a4c61ce180d6af195a23`  
		Last Modified: Wed, 12 May 2021 20:12:36 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ac03dbcc7d806ff532c3c69d7287ef3b4bb4cca73d539ae1662af62799f672e`  
		Last Modified: Wed, 12 May 2021 20:12:36 GMT  
		Size: 1.3 KB (1280 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
