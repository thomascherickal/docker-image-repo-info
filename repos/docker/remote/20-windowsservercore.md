## `docker:20-windowsservercore`

```console
$ docker pull docker@sha256:2e56673109170f38a9ea23b63e4520cccd59182eb26b7c3e3f7a9f6232d2ea6b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 2
	-	windows version 10.0.20348.1006; amd64
	-	windows version 10.0.17763.3406; amd64

### `docker:20-windowsservercore` - windows version 10.0.20348.1006; amd64

```console
$ docker pull docker@sha256:885c7dd83ae73d5516ae58d8f81c06ba2f09de35af42e231fd7f410fd5dc67ce
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2402183352 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:afcb440f5315a166071ed008913ce12108f7399c981f6795b54c736d97b57ecf`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:12:09 GMT
RUN Apply image 10.0.20348.643
# Thu, 08 Sep 2022 20:30:55 GMT
RUN Install update 10.0.20348.1006
# Wed, 14 Sep 2022 12:09:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Sep 2022 19:33:19 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 14 Sep 2022 19:36:25 GMT
ENV DOCKER_VERSION=20.10.18
# Wed, 14 Sep 2022 19:36:26 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.18.zip
# Wed, 14 Sep 2022 19:36:57 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:97f65a0ec59e643faf84024aa713a9be059322380315fda829756bbbd96d6258`  
		Size: 1.4 GB (1436863614 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4486102fd3820ed9527fa3e7bfefa8305c2f054e65b46dffe9675755e3d8f288`  
		Size: 910.1 MB (910085953 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c5da8902b0918fe9bb0d466157622ccaf8209e4becbdd188ec41ecb563c068e6`  
		Last Modified: Wed, 14 Sep 2022 12:41:36 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:334c776d6184fec7acdb5027a6d95b32539f4d420e4b1abe401347adb7cc7377`  
		Last Modified: Wed, 14 Sep 2022 19:39:00 GMT  
		Size: 591.0 KB (591032 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a96865f35f15e88cdd5f10fd3cc53ea7c002e278df70ebc4e3a2da24bf3e4670`  
		Last Modified: Wed, 14 Sep 2022 19:39:27 GMT  
		Size: 1.4 KB (1445 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4d650896bb96a5e18321c44ec07c8d0fc1d6351eb59b98e3dbc6bada76cb3152`  
		Last Modified: Wed, 14 Sep 2022 19:39:27 GMT  
		Size: 1.4 KB (1432 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4c65a9e8fb0af2a97486c3cbf3a394ed6065f82267beca94b98ddd043c97ff10`  
		Last Modified: Wed, 14 Sep 2022 19:39:37 GMT  
		Size: 54.6 MB (54638439 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `docker:20-windowsservercore` - windows version 10.0.17763.3406; amd64

```console
$ docker pull docker@sha256:33d0c4b2cafcf75dba7ac318dd6c542cdbc73a9f559a5e0c73dd513648ecd7e1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2758343788 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:4cbe673467cc5eb962c5825c329436099c334c25058580a80e1c6a1ce1165109`
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
# Wed, 14 Sep 2022 19:37:04 GMT
ENV DOCKER_VERSION=20.10.18
# Wed, 14 Sep 2022 19:37:04 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.18.zip
# Wed, 14 Sep 2022 19:38:13 GMT
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
	-	`sha256:1cd3ae578b4f31ecd9c27bbe3ccdc4d3fd6cb765480e973de4cb87bff28406b5`  
		Last Modified: Wed, 14 Sep 2022 19:39:51 GMT  
		Size: 1.4 KB (1370 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:afbdefbb6a211f6970380dffd709e9339443c674d2b35f3924fbac9c7080dbaf`  
		Last Modified: Wed, 14 Sep 2022 19:39:51 GMT  
		Size: 1.4 KB (1413 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dc42b1e9222f1818e6868d67c6e772757cab99f6ff9e365e848793b7da7d7c4f`  
		Last Modified: Wed, 14 Sep 2022 19:40:00 GMT  
		Size: 54.4 MB (54428942 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
