## `nats-streaming:windowsservercore`

```console
$ docker pull nats-streaming@sha256:69bb9da460900cc4b3c7e7e477ff5647b06d5634739a283fa746fed0de49d79c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3568; amd64

### `nats-streaming:windowsservercore` - windows version 10.0.14393.3568; amd64

```console
$ docker pull nats-streaming@sha256:e69b701f883a5712fc10b1f07be9b87afc2cb5babc7b3bbc1c0ee4d603913453
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.7 GB (5734818179 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c8c4d6dc8aaf76c1ebebb4cf2ce1bd640142b7c6ee9d4f0b54766c6d60a74355`
-	Default Command: `["nats-streaming-server","-m","8222"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Tue, 10 Mar 2020 08:14:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 18 Mar 2020 14:58:05 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 18 Mar 2020 14:58:06 GMT
RUN cmd /S /C #(nop) WORKDIR C:\nats-streaming-server
# Wed, 18 Mar 2020 14:58:07 GMT
RUN cmd /S /C #(nop) COPY file:d30725f7225d14fba35e88513adf63da18fc9fef9c4f6c817dff8f784f19a7c1 in nats-streaming-server.exe 
# Wed, 18 Mar 2020 14:58:09 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 18 Mar 2020 14:58:10 GMT
RUN cmd /S /C #(nop)  CMD ["nats-streaming-server" "-m" "8222"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a5d20b7a2294a0d2631f74f49fc34574484a692913559546ef0bceae789fd7a8`  
		Size: 1.7 GB (1658775203 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:3c743cfa8b7e367517b526c4457b464dacb6ffd65bd231e7d847f44dd76a1ebf`  
		Last Modified: Wed, 18 Mar 2020 14:58:25 GMT  
		Size: 1.1 KB (1129 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:786773aa5e1b848824b0974d77fde1cce8f3f83f1e96716c3d746ed31553f750`  
		Last Modified: Wed, 18 Mar 2020 14:58:25 GMT  
		Size: 1.3 KB (1338 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c6e25625b6d294ee7fc88f677cb1364350aca616ac4ee2c9bd0d957d914d87d9`  
		Last Modified: Wed, 18 Mar 2020 14:58:26 GMT  
		Size: 6.1 MB (6052318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ad29b746e59ca26c22c433d1e362831082ed3766b488ff38b6a87c3b23f84ecd`  
		Last Modified: Wed, 18 Mar 2020 14:58:25 GMT  
		Size: 1.1 KB (1144 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5655e6789b99c7161d4d1975e609bc34751f8c7643fdb794a8b8847fa551acf2`  
		Last Modified: Wed, 18 Mar 2020 14:58:25 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
