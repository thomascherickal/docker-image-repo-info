## `influxdb:meta`

```console
$ docker pull influxdb@sha256:22c88eae3fbd94af0e982672dd26d5374fcdf33eb1b3db1c3cfd52f40793b9e4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	linux; amd64

### `influxdb:meta` - linux; amd64

```console
$ docker pull influxdb@sha256:387338297f9c5dc74b01465f48bc5e128bab7dca396cd1c0fe77e7d3edd98aca
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **94.5 MB (94502250 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:76221c695d2931a543e59540e111c66b7b22073ce1a162bd77b791f8c38eed66`
-	Entrypoint: `["\/entrypoint.sh"]`
-	Default Command: `["influxd-meta"]`

```dockerfile
# Tue, 04 Oct 2022 23:26:27 GMT
ADD file:d1268789456d2cdace6e50149e60404ad5a849b7c61e8fc8bc7b6e0eb6eeb7ca in / 
# Tue, 04 Oct 2022 23:26:27 GMT
CMD ["bash"]
# Wed, 05 Oct 2022 00:54:53 GMT
RUN set -eux; 	apt-get update; 	apt-get install -y --no-install-recommends 		ca-certificates 		curl 		netbase 		wget 	; 	rm -rf /var/lib/apt/lists/*
# Wed, 05 Oct 2022 00:55:00 GMT
RUN set -ex; 	if ! command -v gpg > /dev/null; then 		apt-get update; 		apt-get install -y --no-install-recommends 			gnupg 			dirmngr 		; 		rm -rf /var/lib/apt/lists/*; 	fi
# Wed, 05 Oct 2022 22:56:45 GMT
RUN set -ex &&     mkdir ~/.gnupg;     echo "disable-ipv6" >> ~/.gnupg/dirmngr.conf;     for key in         05CE15085FC09D18E99EFB22684A14CF2582E0C5 ;     do         gpg --keyserver hkp://keyserver.ubuntu.com --recv-keys "$key" ;     done
# Wed, 05 Oct 2022 22:56:56 GMT
ENV INFLUXDB_VERSION=1.8.10-c1.8.10
# Wed, 05 Oct 2022 22:57:19 GMT
RUN wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc &&     wget --no-verbose https://dl.influxdata.com/enterprise/releases/influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     gpg --batch --verify influxdb-meta_${INFLUXDB_VERSION}_amd64.deb.asc influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     dpkg -i influxdb-meta_${INFLUXDB_VERSION}_amd64.deb &&     rm -f influxdb-meta_${INFLUXDB_VERSION}_amd64.deb*
# Wed, 05 Oct 2022 22:57:19 GMT
COPY file:5d8d1b0acfd7ca05cf6698246b28d240206fa448f4aa5ac839c9ad323adbeac2 in /etc/influxdb/influxdb-meta.conf 
# Wed, 05 Oct 2022 22:57:19 GMT
EXPOSE 8091
# Wed, 05 Oct 2022 22:57:19 GMT
VOLUME [/var/lib/influxdb]
# Wed, 05 Oct 2022 22:57:19 GMT
COPY file:126b1f7e41b4975cf2ce23037cf6a46253fb817023062317380c48ff5df47228 in /entrypoint.sh 
# Wed, 05 Oct 2022 22:57:19 GMT
ENTRYPOINT ["/entrypoint.sh"]
# Wed, 05 Oct 2022 22:57:19 GMT
CMD ["influxd-meta"]
```

-	Layers:
	-	`sha256:f606d8928ed378229f2460b94b504cca239fb906efc57acbdf9340bd298d5ddf`  
		Last Modified: Tue, 04 Oct 2022 23:30:27 GMT  
		Size: 55.0 MB (55046248 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:47db815c6a4547dc224b75222193cb1851cf529d2cbdf26f854b9bbf97099b98`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 5.2 MB (5163279 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:bf48494000001a037b72870d2a6a2536f9da8bc5d1ceddd72d79f4a51fe7a60e`  
		Last Modified: Wed, 05 Oct 2022 01:19:13 GMT  
		Size: 10.9 MB (10876505 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc344889471b2f3a92c68a5f31b14f94dfb281995eeb74ab1066e3b615e23ee`  
		Last Modified: Wed, 05 Oct 2022 22:59:38 GMT  
		Size: 2.9 KB (2898 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f114ef9e7ec26af4cd23a5e1804319b53b2e87e39f71e28d6696d9b216b148d`  
		Last Modified: Wed, 05 Oct 2022 23:00:21 GMT  
		Size: 23.4 MB (23412749 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e600061bd76898dc8b3d570e9ce0475fc7f833b63118056e5bea2e29807495a`  
		Last Modified: Wed, 05 Oct 2022 23:00:18 GMT  
		Size: 197.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:65e91464551dde9184822f6b3c93167abef3e0585cc407aabab18f9fafa0bc8c`  
		Last Modified: Wed, 05 Oct 2022 23:00:18 GMT  
		Size: 374.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
