## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:acfd53e7787f2304485e9cb5dbfab73c9e87a9a48bf42e7cbb0004da6eecc0d6
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2928; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.2928; amd64

```console
$ docker pull docker@sha256:31dcdd35e3b51cab21a5e3595b1fb98bc2e0299c78f0429ea0a86c534cf3bab7
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.6 GB (2556828985 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:9049e8afec65e60c04dc8e34f79f883a885aff08b1652374efd8d306439bdf8b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 05 May 2022 17:03:24 GMT
RUN Install update 10.0.17763.2928
# Tue, 10 May 2022 17:40:47 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 May 2022 01:17:07 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 May 2022 01:17:08 GMT
ENV DOCKER_VERSION=20.10.15
# Wed, 11 May 2022 01:17:09 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.15.zip
# Wed, 11 May 2022 01:18:09 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:8b534d64a7c337eb8a23b425e4f598cd3e7407ddf8c7b2f714d1e7f7ed6a04be`  
		Size: 626.9 MB (626889777 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c8a0a0d5642a312541382f8fd8cc5463eea7b9c29d4f71cd1c2592aa0e22160e`  
		Last Modified: Tue, 10 May 2022 18:17:19 GMT  
		Size: 1.4 KB (1428 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6b919bb58ec3ed41b7e2e67e75497f0619d0f5ffa4ed0bf076d25d167186aed5`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 486.0 KB (486016 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:60be3898d881db4d601a12aafc54eec7c0dfece1dca6bbd49a9b83d8960fd9b1`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:49d94933d82ab878efa8b78e97811840e787dfd21efb94ad17dbecaa40f6a93d`  
		Last Modified: Wed, 11 May 2022 01:19:58 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ed3878d883ad2ec89939898edcd7a6861bb777c5a24b7563d515b0e4929191eb`  
		Last Modified: Wed, 11 May 2022 01:20:51 GMT  
		Size: 52.3 MB (52282860 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
