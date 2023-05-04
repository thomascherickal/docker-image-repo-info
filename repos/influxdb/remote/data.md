## `influxdb:data`

```console
$ docker pull influxdb@sha256:ca98b623d9512ed8ed9274058d4e078109f07fc55f143ff3511a9d41af6692cc
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:data` - linux; amd64

```console
$ docker pull influxdb@sha256:9d884ada1b799a356c9ffcaa53aa2914fd8c5a1cfe5be6f80abbd7e330d6bf10
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **127.5 MB (127518125 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1538bfce69e3dc5bb370450b2ce9d78c643f50898c50b5e43e686d706527d5fc`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd"]`

```dockerfile
# Tue, 02 May 2023 23:46:50 GMT
ADD file:fc290cf8ddb984325474583faa79c5a98c5ea0ec7f606bf360251f63acecf389 in / 
# Tue, 02 May 2023 23:46:51 GMT
CMD ["bash"]
# Wed, 03 May 2023 19:58:13 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		gnupg 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Thu, 04 May 2023 10:55:13 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         9D539D90D3328DC7D6C8D3B9D8FF8E1F7DF8B07E ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Thu, 04 May 2023 10:55:22 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Thu, 04 May 2023 10:55:30 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-data_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-data_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-data_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 04 May 2023 10:55:30 GMT
COPY file:bf2f42b62a32a7ee3ab93d9a5e451b7d59af1a97e40dc4a76b8aaf2f64383d7a in /etc/influxdb/influxdb.conf 
# Thu, 04 May 2023 10:55:30 GMT
EXPOSE 8086
# Thu, 04 May 2023 10:55:30 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:55:30 GMT
COPY file:182a0176834db40043100d082d05e5aded9887c94b02416f6e3154c827c07360 in /entrypoint.sh 
# Thu, 04 May 2023 10:55:30 GMT
COPY file:e7af69cde81ffb6eddc175488941183d1244772c36c27b74751d54389fb71701 in /init-influxdb.sh 
# Thu, 04 May 2023 10:55:30 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:55:30 GMT
CMD ["influxd"]
```

-	Layers:
	-	`sha256:918547b9432687b1e1d238e82dc1e0ea0b736aafbf3c402eea98c6db81a9cb65`  
		Last Modified: Tue, 02 May 2023 23:49:58 GMT  
		Size: 55.0 MB (55049070 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5d79063a01c561833dc6546d4e647fda0121a59e1a9a17874a3e30854555475e`  
		Last Modified: Wed, 03 May 2023 20:13:04 GMT  
		Size: 15.8 MB (15760340 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a8e9798c2a3fe481dd78cda51df69e0046dc8e97a398916c12663b9342e3e700`  
		Last Modified: Thu, 04 May 2023 10:56:29 GMT  
		Size: 1.8 KB (1805 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28ad4359c5f3d8340b96395986520fd3a347167a51b7033e3415ca92b76cf7b1`  
		Last Modified: Thu, 04 May 2023 10:56:52 GMT  
		Size: 56.7 MB (56705136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:905dcfeb634b16d5b59f824b3d967725f2e95ad71d0ca7edec1101625fe6f005`  
		Last Modified: Thu, 04 May 2023 10:56:45 GMT  
		Size: 242.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32d9fad405d2820272db336a50bae1d55e209c05db0b62e569db1bfcc3e7cecc`  
		Last Modified: Thu, 04 May 2023 10:56:45 GMT  
		Size: 251.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:000dd25bf5c3dd19ffcb1235ebc0243195891dba177dadda8430f6d6b4a2e330`  
		Last Modified: Thu, 04 May 2023 10:56:45 GMT  
		Size: 1.3 KB (1281 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
