## `nats:nanoserver`

```console
$ docker pull nats@sha256:85c4a376719c9196a006e8695e5b71d53646b96932dabe3da2300383614bc965
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2237; amd64

### `nats:nanoserver` - windows version 10.0.17763.2237; amd64

```console
$ docker pull nats@sha256:7680106cba849c2a69d67a28a303e06cb67ddf69a180b01e3d9a95d0dd3d5e10
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **107.3 MB (107298446 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b1e148bc6290eb593e260bd96ff426067e9093d7a0f079b5f4b0b48df8d163a2`
-	Entrypoint: `["C:\\nats-server.exe"]`
-	Default Command: `["--config","nats-server.conf"]`

```dockerfile
# Thu, 07 Oct 2021 08:01:14 GMT
RUN Apply image 1809-amd64
# Wed, 13 Oct 2021 00:39:10 GMT
RUN cmd /S /C #(nop)  ENV NATS_DOCKERIZED=1
# Fri, 05 Nov 2021 01:16:45 GMT
RUN cmd /S /C #(nop) COPY file:d04f5d85a8b0edde975ace8d01e615862e9872904d6e700eb5be4601ac26087b in C:\nats-server.exe 
# Fri, 05 Nov 2021 01:16:46 GMT
RUN cmd /S /C #(nop) COPY file:bef66f144841968228eb6875fdca1fb9c094da90455a3e05090bdd09e690e7ea in C:\nats-server.conf 
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  EXPOSE 4222 6222 8222
# Fri, 05 Nov 2021 01:16:47 GMT
RUN cmd /S /C #(nop)  ENTRYPOINT ["C:\\nats-server.exe"]
# Fri, 05 Nov 2021 01:16:48 GMT
RUN cmd /S /C #(nop)  CMD ["--config" "nats-server.conf"]
```

-	Layers:
	-	`sha256:934e212983f208dc2bebc5de38259a6a62f1761868aacfee2cb3585a13b1e24b`  
		Size: 102.7 MB (102661372 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6ce10b72796b60d4a0a54a59d8fb8a4f192105fd12bfd7ec08adf49f2c3b159b`  
		Last Modified: Wed, 13 Oct 2021 00:43:58 GMT  
		Size: 1.1 KB (1137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32cd1eaa96684b926e0e43331b86eaa27924b54ed6de221bbf60d9477b4f267b`  
		Last Modified: Fri, 05 Nov 2021 01:20:23 GMT  
		Size: 4.6 MB (4630743 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c8c6070855deac9c75eeec85d14855f1697622fb7fe83c70dd9cef248fbc7743`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.7 KB (1740 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85ac6a75c51fcc7b89b6e0ad03ec3beb67f6392ca758f97509e01d10cc3c5868`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1159 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9bbde88dc838cdb889d5662d53f6df751fcfcc29c4f364e2dd02edafa44e7d66`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.1 KB (1142 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5db2c76db930a9738c89c76236e25feb23aa153e276989e16df1ed0d383900ca`  
		Last Modified: Fri, 05 Nov 2021 01:20:22 GMT  
		Size: 1.2 KB (1153 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
