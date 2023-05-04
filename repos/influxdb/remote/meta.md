## `influxdb:meta`

```console
$ docker pull influxdb@sha256:1818dc3a1014ff8bc213b5c5c681328888abec46f3d4474e5135bee3b70d6f36
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:f0603d40ad7756af805eab578df632b498915815db7c4a5cbfcb3da0bb3df3ba
```

-	Docker Version: 20.10.23
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.2 MB (94224599 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:6fe6dc3badf2bd640104ad7f14bf852f0f9f759cf005ab0204d363bf28060ad5`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

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
# Thu, 04 May 2023 10:55:37 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Thu, 04 May 2023 10:55:37 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Thu, 04 May 2023 10:55:37 GMT
EXPOSE 8091
# Thu, 04 May 2023 10:55:37 GMT
VOLUME [/var/lib/influxdb]
# Thu, 04 May 2023 10:55:38 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Thu, 04 May 2023 10:55:38 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Thu, 04 May 2023 10:55:38 GMT
CMD ["influxd-meta"]
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
	-	`sha256:a0368ac17311eed9aa2f8af4609296812671e408e74467e8a3780f1b6c96647f`  
		Last Modified: Thu, 04 May 2023 10:57:05 GMT  
		Size: 23.4 MB (23412812 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:957182bf465a16a9c61a29d31942940468a7088fdf3edc6bc6fb48df5c0668e0`  
		Last Modified: Thu, 04 May 2023 10:57:02 GMT  
		Size: 198.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:756b9e95001e2a1351853e2c1fe60b068c14e181fd926b78f4d49961880c71ee`  
		Last Modified: Thu, 04 May 2023 10:57:02 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
