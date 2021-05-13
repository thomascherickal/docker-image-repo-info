## `nats-streaming:nanoserver-1809`

```console
$ docker pull nats-streaming@sha256:ec0aed95b5234c5cc882c7be18390dfb68a43a5285973d2264fc7cea404785ba
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1935; amd64

### `nats-streaming:nanoserver-1809` - windows version 10.0.17763.1935; amd64

```console
$ docker pull nats-streaming@sha256:881fbff9b8ea5b5dce5d1e1fb341a4ab9a9caab12b0faf072dc89f9ab61792e9
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.2 MB (107191037 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a9db19cc378f4cdf654406f9ff0a58704fbec29c0b23fa37b4919bcedd9a0a02`
-	Entrypoint: `["C:\\nats-streaming-server.exe"]`
-	Default Command: `["-m","8222"]`

```dockerfile
# Fri, 07 May 2021 11:54:57 GMT
RUN Apply image 1809-amd64
# Wed, 12 May 2021 15:44:03 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Wed, 12 May 2021 20:11:27 GMT
RUN cmd /S /C #(nop) COPY file:adacf7e54ef5a782ae37764b59883ad6a48b32c36c576816360f94cba82ba458 in C:\nats-streaming-server.exe 
# Wed, 12 May 2021 20:11:28 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 8222
# Wed, 12 May 2021 20:11:29 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-streaming-server.exe"]
# Wed, 12 May 2021 20:11:30 GMT
RUN cmd /S /C #(nop)  CMD ["-m" "8222"]
```

-	Layers:
	-	`sha256:b9043d31610e0dfa43b1afe286f8918b6e3bf69ece50f44424b29d48f20aa662`  
		Size: 101.4 MB (101375240 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:95b58e21e5cdf4e2f9e5c87487734458885da325634d72f9c4e6583b353af06f`  
		Last Modified: Wed, 12 May 2021 15:49:02 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ab3056c607d4b35216a2f74c2f849eb0c970001dc87bf45f90aea3ca4e8d9f05`  
		Last Modified: Wed, 12 May 2021 20:16:11 GMT  
		Size: 5.8 MB (5811203 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:747d370e1cec130d4e6c1a20a9b8d049a93543b695b60a4fc0b5473758786920`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1178 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:38d9d67f8ca438fa616690db8fc1087b47f11ad390d7a29761bfc08c67605c85`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.1 KB (1105 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e187a1b2446f3948440517b1cd475bdb32db16b4643b465f30313f8bbfe01d6`  
		Last Modified: Wed, 12 May 2021 20:16:10 GMT  
		Size: 1.2 KB (1161 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
