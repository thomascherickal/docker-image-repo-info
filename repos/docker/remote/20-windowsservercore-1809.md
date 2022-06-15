## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:f8c99a477afebef2e0a504c1a2d40be47010d4e93cb99febe638d0eb20505199
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.3046; amd64

```console
$ docker pull docker@sha256:92b9efc4d05fc727177fa4d4f20e8ca35969778a932858c93dde72a69cafa065
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2715917945 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:208e7e03e3e360a634a05b786e8043476d165cf2930fc4237e9c34c390385228`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 22:48:09 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 15 Jun 2022 22:50:28 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 15 Jun 2022 22:50:29 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 15 Jun 2022 22:51:41 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:be4c7110da70e07b37a00b3b05b18361572412287fee26eba04fcf23dcb75639`  
		Last Modified: Wed, 15 Jun 2022 22:52:48 GMT  
		Size: 352.2 KB (352228 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7a3fc52e3c402b1be6f7512b16405aaaba3edd6037ede2a7885b367bec19efd`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1418 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:92deca7aa7a34f968926e81414d0102042c2a2e85968fa9423cb1ceed71a9393`  
		Last Modified: Wed, 15 Jun 2022 22:53:28 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f346f796df4e8cb918a2d6f83dcf31d1544d3af9b283727e9757400a160423ab`  
		Last Modified: Wed, 15 Jun 2022 22:53:39 GMT  
		Size: 52.3 MB (52281684 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
