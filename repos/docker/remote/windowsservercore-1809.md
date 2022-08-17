## `docker:windowsservercore-1809`

```console
$ docker pull docker@sha256:053cc56fb3493790eeae1ff6ee7b9af43a55425247602f183ffc4056467e6d46
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3287; amd64

### `docker:windowsservercore-1809` - windows version 10.0.17763.3287; amd64

```console
$ docker pull docker@sha256:9f8201aaa5ae59fc28b5fd82b737a093eb7b191066d54000681a804328136ffa
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2730340296 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c9b2f7ade9780d733f10425ef24e89268ceb907ff0c616eb5657ebe3a6007236`
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
# Wed, 10 Aug 2022 19:19:07 GMT
ENV DOCKER_VERSION=20.10.17
# Wed, 10 Aug 2022 19:19:08 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.17.zip
# Wed, 10 Aug 2022 19:20:10 GMT
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
	-	`sha256:32032f8b3b426b3d8d284cd7c4ccc3c1b218598434dd588d0645b2d6f34b0684`  
		Last Modified: Wed, 17 Aug 2022 01:16:38 GMT  
		Size: 1.3 KB (1326 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e86c8df3508096f8a4674b523ae9a635928f0e995f52657f19993c4c9e73bfaf`  
		Last Modified: Wed, 17 Aug 2022 01:16:38 GMT  
		Size: 1.3 KB (1290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2c11bf19233c605630e1821cfd6de92e3bc7dca5dfed134e2c586a2dda021a70`  
		Last Modified: Wed, 17 Aug 2022 01:16:48 GMT  
		Size: 52.3 MB (52278879 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
