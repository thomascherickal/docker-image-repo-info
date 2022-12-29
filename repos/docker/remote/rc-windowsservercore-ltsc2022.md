## `docker:rc-windowsservercore-ltsc2022`

```console
$ docker pull docker@sha256:e941313c2adfcae195333d3f35e13adb0fd095e390d31440caf69e72ce9c6fe6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.1366; amd64

### `docker:rc-windowsservercore-ltsc2022` - windows version 10.0.20348.1366; amd64

```console
$ docker pull docker@sha256:9c8f7a211fd9dac7641ad5e2f0e1b7de9fa070c08764954a75e3bb004f9808de
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.5 GB (2513742221 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:16053ff94653594a80c549e5071b8b1123221417ab9b9f27e0ce5236ff3ccd5b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Fri, 09 Dec 2022 09:36:47 GMT
RUN Install update 10.0.20348.1366
# Tue, 13 Dec 2022 22:45:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Dec 2022 03:16:32 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 29 Dec 2022 17:15:49 GMT
ENV DOCKER_VERSION=23.0.0-rc.1
# Thu, 29 Dec 2022 17:15:51 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-23.0.0-rc.1.zip
# Thu, 29 Dec 2022 17:16:47 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:a4aee932fccc1ec8135f290aca03a7c93dcc2536fc84723813ef9b95f6fd13ea`  
		Last Modified: Wed, 18 May 2022 07:59:24 GMT  
		Size: 1.5 GB (1473997635 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3bfa20ce142ecceb471dc070d9582fff942cef447b7c8ff22f2223ffe3737c99`  
		Last Modified: Tue, 13 Dec 2022 23:54:14 GMT  
		Size: 1.0 GB (1021665190 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7eb8b9a4ec3ca516cfaa44f64e80b1e3aaecdbde870177411ff046f81f991dd2`  
		Last Modified: Tue, 13 Dec 2022 23:51:33 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f9d034b6762cd43683e1a06d639dc882ef3570cd611b77a89c8394fafaf65fe`  
		Last Modified: Wed, 14 Dec 2022 03:24:23 GMT  
		Size: 574.5 KB (574465 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f0be943622b2ad2a337625e75ce6be58433a52fe12ed197a466f07830d8848cb`  
		Last Modified: Thu, 29 Dec 2022 17:19:37 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:515d692f07e3e06cb18447f597562f6111df955ff1a3b1804d02e03ce703d92d`  
		Last Modified: Thu, 29 Dec 2022 17:19:37 GMT  
		Size: 1.4 KB (1417 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:512d3379f382d812ce3fda424806c1eefb4d00adffc8a18b1eb580b12b2f5533`  
		Last Modified: Thu, 29 Dec 2022 17:19:41 GMT  
		Size: 17.5 MB (17500659 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
