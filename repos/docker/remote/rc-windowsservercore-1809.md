## `docker:rc-windowsservercore-1809`

```console
$ docker pull docker@sha256:5e3ef4617547fa64fed008f3db789e840df85ecd9487fd9fe3c9f6d809f56cdf
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3770; amd64

### `docker:rc-windowsservercore-1809` - windows version 10.0.17763.3770; amd64

```console
$ docker pull docker@sha256:31cd62911daf1214fe63a8085e80a6f4df9ea9b6d9c000587f6de421acc4d252
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2798356924 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:129eff407badd32b0fc87bf410bcc08978faabda89e4b91767ea61272d8e6661`
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
# Thu, 29 Dec 2022 17:16:58 GMT
ENV DOCKER_VERSION=23.0.0-rc.1
# Thu, 29 Dec 2022 17:17:05 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-23.0.0-rc.1.zip
# Thu, 29 Dec 2022 17:18:45 GMT
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
	-	`sha256:63f4eb68e53dc41a506d002a0e56b0b19d0d9a6da7512c941e84597a41dd9df4`  
		Last Modified: Thu, 29 Dec 2022 17:19:51 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8eeebe3a2f344b1dbacc8d44289fac786c61fda06de8d19631d0f63c50690f68`  
		Last Modified: Thu, 29 Dec 2022 17:19:51 GMT  
		Size: 1.4 KB (1352 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6421b6e77a45d4e88b51621d993457545a38e28981938cbd6d0090c451397b4b`  
		Last Modified: Thu, 29 Dec 2022 17:19:54 GMT  
		Size: 17.3 MB (17309941 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
