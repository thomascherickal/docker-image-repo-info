## `docker:rc-windowsservercore-1809`

```console
$ docker pull docker@sha256:0a7cef55d662ab315b45632bfcec30bb712cea66bafc99a3949783e4d85adaaa
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3406; amd64

### `docker:rc-windowsservercore-1809` - windows version 10.0.17763.3406; amd64

```console
$ docker pull docker@sha256:ea5f2f34ef848eff2a0c3c859ee1aac264976d98a70f07050c8e9ccb0a9fcec5
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2713439893 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:538ed6a08c8eb9ded044b3ba09b3b8fd430450a6cea787c7b46d2df59ed88cad`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Fri, 09 Sep 2022 22:43:02 GMT
RUN Install update 10.0.17763.3406
# Tue, 13 Sep 2022 18:21:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 19:35:00 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Sep 2022 19:35:01 GMT
ENV DOCKER_VERSION=22.06.0-beta.0
# Wed, 14 Sep 2022 19:35:01 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/test/x86_64/docker-22.06.0-beta.0.zip
# Wed, 14 Sep 2022 19:36:05 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:cee64bf279e2ca8e924884a10ecb98bfa79c7f0cc8d25e73039b9aeb940815b6`  
		Size: 826.4 MB (826398623 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2bc395c8c47e61e593d2e905e0e051d40e7d25e4aeac7dbe08d3ec57acd0e68f`  
		Last Modified: Tue, 13 Sep 2022 18:25:24 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6729738068cf65fb2e7df0b27735fcc08b65d92d97627f2644e0d90821247e52`  
		Last Modified: Wed, 14 Sep 2022 19:39:14 GMT  
		Size: 345.9 KB (345922 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2709cf758bc23a6cc53f96c5f30e95023b240b5cc75a100381eaa1c63148ba6`  
		Last Modified: Wed, 14 Sep 2022 19:39:13 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:27053dd07eae74dd30d248eb31c25a6313b5228cc4d392ffdb47a72500cf3df4`  
		Last Modified: Wed, 14 Sep 2022 19:39:13 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8ed615fa683414653bfa52e83f1c6fe8e90195037ec246ad5e5696cca63e5634`  
		Last Modified: Wed, 14 Sep 2022 19:39:16 GMT  
		Size: 9.5 MB (9525009 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
