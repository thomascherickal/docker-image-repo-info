## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:916c386ed8189a8cd63b0c83e9a7f66447b0e3659c1c96fa6015589344c723b5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:053a4ca3955b9c5036e48bafb96c83003fe86c34c6928934e3fd1db0529a889c
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.5 MB (6487259 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:993a204b53252cabfc16952c1d2dc014dc6518d1a08d00bda1bc5008a139e37a`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:33:13 GMT
COPY file:3ed83d1497b0535960e452435cb8b27e347f48da12693aa27ebaf9bff94d82de in /nats-streaming-server 
# Tue, 03 Nov 2020 00:33:13 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:33:14 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:33:14 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:57ac21f890a508f609eabea265197b18ce9dfe3e694034c7a06d37b536a707b2`  
		Last Modified: Tue, 03 Nov 2020 00:33:37 GMT  
		Size: 6.5 MB (6487259 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:bbb3d771f9232932017b9cb9b501734367bc3560eed790695be682d94a8f3573
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5444243 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4ed880c2955fd126b0ce38471e90c9467c9c739f55b4c789cec1a4575a41d36f`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:53:53 GMT
COPY file:617b9b5366d0d437ce471ad0763bdd7d350496612583dc2c7044dcde4d32257e in /nats-streaming-server 
# Mon, 11 Jan 2021 23:53:54 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:53:54 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:53:55 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7cffcff2c5b4913dac660d7456365492a0393b1aa6f1812f6b7b46b250e1970d`  
		Last Modified: Mon, 11 Jan 2021 23:54:39 GMT  
		Size: 5.4 MB (5444243 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v7

```console
$ docker pull nats-streaming@sha256:5fd0943909d8aedafb888e099c9f64d234023ad780805ed7c939692ebfd8304d
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6043163 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f37071e856ae40dc3c8c5e10b359d1640fd67a6110741c0957af2031032ed6ce`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Tue, 03 Nov 2020 00:05:23 GMT
COPY file:d232132ddff1d85d3a2f5c80a91c80023cbc103d816387e06d604cf97238e52c in /nats-streaming-server 
# Tue, 03 Nov 2020 00:05:24 GMT
EXPOSE 4222 8222
# Tue, 03 Nov 2020 00:05:24 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Tue, 03 Nov 2020 00:05:25 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:9c7227cc1040d04ca7763cfb53ab58bc32ae54921990516adf8e13374ac9ef29`  
		Last Modified: Tue, 03 Nov 2020 00:05:57 GMT  
		Size: 6.0 MB (6043163 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm64 variant v8

```console
$ docker pull nats-streaming@sha256:0f315491d4d14e634f971591c7f8bd0eb9aad59975fcdf867a51294df2e5efb2
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.4 MB (5388538 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:22dba974517468c29a982c1b4a0b7744a93825122145a1dcc5f7e53c96119efa`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 11 Jan 2021 23:47:25 GMT
COPY file:5a251d4e6bafc9d9ea6f25cd37fd44252da405176da94cc580cdd663abecffa5 in /nats-streaming-server 
# Mon, 11 Jan 2021 23:47:26 GMT
EXPOSE 4222 8222
# Mon, 11 Jan 2021 23:47:26 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 11 Jan 2021 23:47:27 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58239a1ea6494e431645c7ad156ed917333a248edbe6be76af8b7384d9339f07`  
		Last Modified: Mon, 11 Jan 2021 23:48:09 GMT  
		Size: 5.4 MB (5388538 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
