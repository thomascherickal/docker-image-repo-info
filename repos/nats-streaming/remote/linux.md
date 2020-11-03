## `nats-streaming:linux`

```console
$ docker pull nats-streaming@sha256:8df5984380dbe779b490ebe2082c1000b06de56790cd3d47be6df854407d3c31
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	linux; amd64
	-	linux; arm variant v6
	-	linux; arm variant v7
	-	linux; arm64 variant v8

### `nats-streaming:linux` - linux; amd64

```console
$ docker pull nats-streaming@sha256:eff8b99b0e3d89b6161ceb975a8c1ca063ac9a8e868eed448736a866551357ca
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 MB (5936411 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:51d28dc2950a94ff3d73d86750b57ba3c6dae964c671dbac699c2f17eecd5880`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Thu, 25 Jun 2020 19:25:44 GMT
COPY file:6241d3a0b9f20d843fc13c1bd49fd4376e4daae879837447249456f65dfe9ead in /nats-streaming-server 
# Thu, 25 Jun 2020 19:25:44 GMT
EXPOSE 4222 8222
# Thu, 25 Jun 2020 19:25:44 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Thu, 25 Jun 2020 19:25:44 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:908e6af6575b3ee0ca4b089b18f72d87607c39809caeee4bb662b347aa23b895`  
		Last Modified: Thu, 25 Jun 2020 19:26:07 GMT  
		Size: 5.9 MB (5936411 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `nats-streaming:linux` - linux; arm variant v6

```console
$ docker pull nats-streaming@sha256:f334d10ef2a4663d8d7d920d96321cd97f050b82a5d55d588192f074f60dd814
```

-	Docker Version: 19.03.12
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.0 MB (6049845 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9eecfd5ab4178a65e952a7cf1d248a556a6ae2c328ac8b68923146d64734db03`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Mon, 02 Nov 2020 23:56:28 GMT
COPY file:d6896b1c93dcd497494c972f9274fcc634a4f4a8d63a0191bdb87f6336aec0d7 in /nats-streaming-server 
# Mon, 02 Nov 2020 23:56:28 GMT
EXPOSE 4222 8222
# Mon, 02 Nov 2020 23:56:29 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Mon, 02 Nov 2020 23:56:29 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:7f165fb71ab77e8081dbfa13656cdf9e5e005002d6c3afa0aac40667a0f97af8`  
		Last Modified: Mon, 02 Nov 2020 23:57:04 GMT  
		Size: 6.0 MB (6049845 bytes)  
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
$ docker pull nats-streaming@sha256:ed524c7b14a4b6e91428f8c765455f742c4351657468296a8b63bdefecd5ceb1
```

-	Docker Version: 18.09.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.5 MB (5469641 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:2424d5ea5176bb2af173ccb2222a5d39ff53c785fdad2bfc1045d5c66aee5185`
-	Entrypoint: `["\/nats-streaming-server"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Wed, 29 Jul 2020 22:40:10 GMT
COPY file:f3f47d8e20155d8cbd02ab8a9f26c3be2763cf0430c38ab1071fb6949f9e466c in /nats-streaming-server 
# Wed, 29 Jul 2020 22:40:11 GMT
EXPOSE 4222 8222
# Wed, 29 Jul 2020 22:40:11 GMT
ENTRYPOINT ["/nats-streaming-server"]
# Wed, 29 Jul 2020 22:40:12 GMT
CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:58414d7c10a2a92ebdcb56bcf4a04f62f2f370c1e415c008fda228ab012a1a45`  
		Last Modified: Wed, 29 Jul 2020 22:40:42 GMT  
		Size: 5.5 MB (5469641 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
