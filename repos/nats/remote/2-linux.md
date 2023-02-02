## `nats:2-linux`

```console
$ docker pull nats@sha256:c926cdb68b698f2bbe658b5dac5353803f29c4cd4e7ab8bdc572077ee8a9f870
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 4
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats:2-linux` - linux; amd64

```console
$ docker pull nats@sha256:b7cd8c3270f038b671b4d55156398eec4387fff96c2de872255d30024bf6a557
```

-	Docker Version: 20.10.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.9 MB (4931647 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b82b64c84efab021cd029f60c01c7e52b53b4eae18827b383f87a4393b3a7095`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:33:01 GMT
COPY file:a9e60c6fbbdd9ebb5d2c4deec1df6db6d6a40a0384a5544b6c3386eea2057a54 in /nats-server 
# Thu, 02 Feb 2023 21:33:02 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:33:02 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:33:02 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:33:02 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:33:02 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:1cd3edd838903059461e505e0f1e09d3452d5e632e2b550f4d0850b0d2f59c72`  
		Last Modified: Thu, 02 Feb 2023 21:33:50 GMT  
		Size: 4.9 MB (4931138 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0e56ba114f2531c68c394372ad404aeb5ac8ee8946fb17af7ac704a76697756f`  
		Last Modified: Thu, 02 Feb 2023 21:33:49 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v6

```console
$ docker pull nats@sha256:c1107d0e00f4d8dedfbf7883fbabc7b200545657e1e13495e12453d13dfde328
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4694918 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8c7de15c41747ca8b98deb9b16e6b45e323bf1b12bfe5ba0617911396006a4fc`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:be32648053f47b33b445bad52bed7ff3e74d1dc77100df4d672e431022428de7 in /nats-server 
# Thu, 02 Feb 2023 21:50:29 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:50:29 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:50:29 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:50:29 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:50:29 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:eddbc6c88066991dd5810d3a3b6875ee06eecb063cccc9b0e3d9386c75c4f826`  
		Last Modified: Thu, 02 Feb 2023 21:52:00 GMT  
		Size: 4.7 MB (4694411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:795c72903a6f36672ee81a0386bff46e30e1f3598c7552f5c192f650d82c6e69`  
		Last Modified: Thu, 02 Feb 2023 21:51:59 GMT  
		Size: 507.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm variant v7

```console
$ docker pull nats@sha256:8a3086f469fd77000e1a8618960b722ca85e5cbd69a41190e81286734c7e455a
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.7 MB (4688297 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:aa7e9966ce4e992db69b98063dd7d35d6fe1239100d385115ea7031b9b65978b`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:a67f587b7b86d3c3a85687c0097c93084fb71c44966695879cd46269a36ed31d in /nats-server 
# Thu, 02 Feb 2023 21:58:12 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:58:12 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:58:12 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:58:12 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:58:12 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:df148ca425b44984356880f1ed4c1f04d36d2e6efa76ba4043d9dd80fe9f6201`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 4.7 MB (4687788 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b679ac38b5a1c67873f0f08c522aafadecaa085bed163dcc8387ddd53c0509d2`  
		Last Modified: Thu, 02 Feb 2023 21:59:43 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats:2-linux` - linux; arm64 variant v8

```console
$ docker pull nats@sha256:b33b08f196a8f9b3b612740d36e847c1d5bc5239bf49f768b0056cd2ff7baaf0
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **4.5 MB (4517074 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:21aad311a08f5e75bd795b33799a8a100d9eb132974428f406329a5871687f79`
-	Entrypoint: `["\/nats-server"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:f1194fd7c754730901a7920f7db8ad6e6432e904adfe27cb3bf09f1626eb0b20 in /nats-server 
# Thu, 02 Feb 2023 21:47:40 GMT
COPY file:2c51166f33066351f3cfe3734f884c41f36fb66575bdde453c5c93e819cfae35 in /nats-server.conf 
# Thu, 02 Feb 2023 21:47:40 GMT
EXPOSE 4222 6222 8222
# Thu, 02 Feb 2023 21:47:40 GMT
ENV PATH=/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/
# Thu, 02 Feb 2023 21:47:40 GMT
ENTRYPOINT ["/nats-server"]
# Thu, 02 Feb 2023 21:47:40 GMT
CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:0e112ba48caecfa7e51d560718ada0f9c4e686bdc09555df0617055a883e5777`  
		Last Modified: Thu, 02 Feb 2023 21:48:28 GMT  
		Size: 4.5 MB (4516565 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fce6348af8f3a9160210d4305f3a6f5c76b1b36d75df166f313f92cf3774f93f`  
		Last Modified: Thu, 02 Feb 2023 21:48:27 GMT  
		Size: 509.0 B  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
