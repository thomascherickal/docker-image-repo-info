## `docker:rc-windowsservercore-1809`

```console
$ docker pull docker@sha256:9c13898da00bcdcb7d2f8e0cd5b636cf0044a26ce4481a8fdbecbfde1c25fbe5
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `docker:rc-windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull docker@sha256:7dd094763a2eb5873fb23126865f40473e48c8c35677dfcc8012d60d4975b540
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2687585200 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:8aed87660091c8d5e82e716bb38ca488913318d896382dcc9e068107fcbc81a0`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 06 Aug 2022 18:30:32 GMT
RUN Install update 10.0.17763.3287
# Wed, 10 Aug 2022 12:16:16 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Aug 2022 19:17:16 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 10 Aug 2022 19:17:16 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Wed, 10 Aug 2022 19:17:17 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-22.06.0-beta.0.zip
# Wed, 10 Aug 2022 19:18:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:294d77ac553d7210b662d07674ef9e39a6c2e88dc15b9d2788d51e509bc8b54e`  
		Size: 800.5 MB (800546641 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d64f32398ff5e4ac4cbab317ffed87a2fbf4e4a37210284dba19f2929d631a95`  
		Last Modified: Wed, 10 Aug 2022 12:42:57 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5010c9f2d7e0951353d9bb92cce15eefcafc02a982074caebc0cd7f103e7b33c`  
		Last Modified: Wed, 17 Aug 2022 01:15:58 GMT  
		Size: 344.6 KB (344642 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ec7106200a8b5c5e305384be45433e82ca0ae0df0e3fe2f306716231d66ccb7c`  
		Last Modified: Wed, 17 Aug 2022 01:15:57 GMT  
		Size: 1.3 KB (1318 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e8a57220db99941dcddb4a4f24782dea6a6e79d8df7cf7bdb898e5856c70c3e9`  
		Last Modified: Wed, 17 Aug 2022 01:15:58 GMT  
		Size: 1.3 KB (1319 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c890c6e4799f9ef99432e58647a35b4c0db2bc95b95b099cd316166f034ee706`  
		Last Modified: Wed, 17 Aug 2022 01:16:01 GMT  
		Size: 9.5 MB (9523762 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
