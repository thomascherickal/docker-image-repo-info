## `hello-world:nanoserver`

```console
$ docker pull hello-world@sha256:5176bd0f39d68ba608e58fa6d6340a897dc57f5536947435ac4103cb0f765a71
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1547; amd64
	-	windows version 10.0.17763.4010; amd64

### `hello-world:nanoserver` - windows version 10.0.20348.1547; amd64

```console
$ docker pull hello-world@sha256:660408e6ce09363b7dc1a30b210e1888bfa4ff7342e7d69e87463d184dc0cbad
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **122.1 MB (122121945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b27964edb003160e8713064c4fb948862a9fd09df36cb1b2769ba3771430ce3a`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Tue, 07 Feb 2023 11:05:29 GMT
RUN Apply image 10.0.20348.1547
# Thu, 16 Feb 2023 00:36:42 GMT
RUN cmd /S /C #(nop) COPY file:ac9f104fd739943f22886335a779468d86b20ac43fd3168171f6b23fc28882b9 in C: 
# Thu, 16 Feb 2023 00:36:43 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:2e8a1636f1721beefd71f8e0c7176faabfe00d7503a69e909468fd63ac3a4992`  
		Last Modified: Thu, 16 Feb 2023 00:30:27 GMT  
		Size: 122.1 MB (122119166 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d2121432de786818baa41c0bc18fe946418959d7da8d8e38bed2ad5a3e068f1e`  
		Last Modified: Thu, 16 Feb 2023 00:37:07 GMT  
		Size: 1.7 KB (1742 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:691bad357f395a72cdf90f92a0d97c97c35935bce93479230fb9a82b42184231`  
		Last Modified: Thu, 16 Feb 2023 00:37:07 GMT  
		Size: 1.0 KB (1037 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `hello-world:nanoserver` - windows version 10.0.17763.4010; amd64

```console
$ docker pull hello-world@sha256:f01c39d7dc9bff6475b855fe3a94a5233955696b3b8090222807010230a553c6
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **106.7 MB (106677829 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:e7c2385a663fe328a753fa44090c644868949b764b64131d792c49a1f28d151a`
-	Default Command: `["cmd","\/C","type C:\\hello.txt"]`

```dockerfile
# Tue, 07 Feb 2023 10:14:28 GMT
RUN Apply image 10.0.17763.4010
# Thu, 16 Feb 2023 00:36:51 GMT
RUN cmd /S /C #(nop) COPY file:994f63bc3cea8285310afa5f4677df29bf99dd4cd1881c7e381100a9e794ba71 in C: 
# Thu, 16 Feb 2023 00:36:52 GMT
RUN cmd /S /C #(nop)  CMD ["cmd" "/C" "type C:\\hello.txt"]
```

-	Layers:
	-	`sha256:00eaf3341cd3cc6b72f91399cb3bd1aba30eb7eead7596532fe54c4bf1b010d7`  
		Last Modified: Thu, 16 Feb 2023 00:31:21 GMT  
		Size: 106.7 MB (106674970 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4196b3ac104db443cc49425d58a29ee18f259c80c4dddf7b847ce40ac796ba83`  
		Last Modified: Thu, 16 Feb 2023 00:37:13 GMT  
		Size: 1.7 KB (1723 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a3c526cc3f7a61b22c5c29e22d8757dff846f5f8b8e1c1d435688942f84456ff`  
		Last Modified: Thu, 16 Feb 2023 00:37:13 GMT  
		Size: 1.1 KB (1136 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
