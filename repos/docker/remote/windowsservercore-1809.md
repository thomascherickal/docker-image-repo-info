## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:5d3b6e0dc8b3fa8dc5bd5eb84b9147e60090ffff34fe8ea2a735b16f129231d4
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull docker@sha256:e90e9f0ccade1a5642a6ce19867bc472fb9411020e2bd37802958fba62b8b148
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2835491264 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:996c0a599fa4ebda5474612f525eab5ce6341c65452108dab719365f4c9f959f`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sun, 11 Dec 2022 08:04:49 GMT
RUN Install update 10.0.17763.3770
# Tue, 13 Dec 2022 22:48:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Dec 2022 03:19:03 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Dec 2022 03:21:56 GMT
ENV DOCKER_VERSION=20.10.21
# Wed, 14 Dec 2022 03:21:57 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.21.zip
# Wed, 14 Dec 2022 03:23:38 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f3ad73ed772f80ab7923579a55dd12fb9b6e090d1d836408d16ffd9d3dee252`  
		Last Modified: Tue, 13 Dec 2022 23:56:47 GMT  
		Size: 856.4 MB (856427878 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0bc9debb9503ac53c2f64685982eca56ac5110ea6baf7278b27af54ab8fbc409`  
		Last Modified: Tue, 13 Dec 2022 23:54:25 GMT  
		Size: 1.4 KB (1435 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85b9e2f22bf688283deaef6ed97938c8cd47d221a71f33d32c1727fbce062fd9`  
		Last Modified: Wed, 14 Dec 2022 03:24:37 GMT  
		Size: 345.6 KB (345581 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed1c373c20aa2631f405bb98c4449019cd7192ef1df699b90ea13c8c2cdcd2e8`  
		Last Modified: Wed, 14 Dec 2022 03:25:16 GMT  
		Size: 1.4 KB (1441 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f1e6f465a2ca4dfe107dbc3c63d62de049fc0aeefa46e585115e2d138c0f038f`  
		Last Modified: Wed, 14 Dec 2022 03:25:16 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1557f8a8145b8240eb510e4bb3ffbef4ee82e0c3671a1bb5ceb657b0ae5dc844`  
		Last Modified: Wed, 14 Dec 2022 03:25:27 GMT  
		Size: 54.4 MB (54444137 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
