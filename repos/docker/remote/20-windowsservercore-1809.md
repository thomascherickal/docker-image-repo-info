## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:a5f651483ed96a2f0b84a50a66bb82ffd53cb16b7bb6d8db9fb2fde6e080d3a1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3650; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.3650; amd64

```console
$ docker pull docker@sha256:9c58d231789d85406c8f9457cc6106db3f28a6a6dcd7c4cfcc5dbb3e24c38191
```

-	Docker Version: 20.10.21
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2833403036 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:a7aee76ebe10a5a950ed2f33f597ad44e41156f350dd136798a995ed8479ada9`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 05 Nov 2022 18:29:26 GMT
RUN Install update 10.0.17763.3650
# Tue, 08 Nov 2022 18:31:26 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Nov 2022 19:32:16 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 09 Nov 2022 19:34:38 GMT
ENV DOCKER_VERSION=20.10.21
# Wed, 09 Nov 2022 19:34:40 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.21.zip
# Wed, 09 Nov 2022 19:36:04 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:a48a3e4ae2de839d8e99bde16eb91d113fb2cf889bba472d0c4274851b5fb402`  
		Last Modified: Tue, 21 Jun 2022 18:30:17 GMT  
		Size: 1.9 GB (1924269350 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c26cc6e4f9eb1ae415a5ead6f884cac597bbd57efa6cd042c878d5b54c9d2091`  
		Last Modified: Tue, 08 Nov 2022 19:44:35 GMT  
		Size: 854.3 MB (854317461 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f182832ad6ad5ea3d4b7320fd7bfea56fb9cf8413be904e52db6ed14c8d9e36f`  
		Last Modified: Tue, 08 Nov 2022 19:42:07 GMT  
		Size: 1.4 KB (1440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:52f4400d25d870dc67fb4609bfa712ae26190577079be89f8156d6666b3decac`  
		Last Modified: Wed, 16 Nov 2022 14:55:55 GMT  
		Size: 363.3 KB (363314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:174d538e9504e5103eae088078327a9f4e21ae830fe7964cf2b9435f91b05ed7`  
		Last Modified: Wed, 16 Nov 2022 14:56:38 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2883faf80801f4c02c1b6ef877ba7084bbeeec7ed6a45ba8d3e4664836e78b64`  
		Last Modified: Wed, 16 Nov 2022 14:56:37 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5f28635d095bd0157d75e2b15ff8925257b785a6eb0dcd7923bddbf992b18d28`  
		Last Modified: Wed, 16 Nov 2022 14:56:53 GMT  
		Size: 54.4 MB (54448631 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
