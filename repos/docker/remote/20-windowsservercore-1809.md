## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:09c96e129b7a6f7fe87fa9fcf92d6232f2ccb71179c5658d564f1a66baaa69f3
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull docker@sha256:9fe6bca6f4fcaf3659519550bd4659a85da6dfe310e48101082337dd56b80245
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2765948023 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c7c9e47705bd0c998596b755f8dcdb2b448160577abdeb79e8af308a0821d7a6`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Sat, 08 Oct 2022 01:55:32 GMT
RUN Install update 10.0.17763.3532
# Tue, 11 Oct 2022 20:24:02 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 12 Oct 2022 18:09:38 GMT
RUN $newPath = ('{0}\docker;{1}' -f $env:ProgramFiles, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Thu, 13 Oct 2022 23:23:54 GMT
ENV DOCKER_VERSION=20.10.19
# Thu, 13 Oct 2022 23:23:55 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.19.zip
# Thu, 13 Oct 2022 23:25:14 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:DOCKER_URL); 	Invoke-WebRequest -Uri $env:DOCKER_URL -OutFile 'docker.zip'; 		Write-Host 'Expanding ...'; 	Expand-Archive docker.zip -DestinationPath $env:ProgramFiles; 		Write-Host 'Removing ...'; 	Remove-Item @( 			'docker.zip', 			('{0}\docker\dockerd.exe' -f $env:ProgramFiles) 		) -Force; 		Write-Host 'Verifying install ("docker --version") ...'; 	docker --version; 		Write-Host 'Complete.';
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:028c482fad0f111537a40f65401f65de54c9fd682951a4f8cf9b644d7c128e18`  
		Size: 834.0 MB (833997855 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c70f9828a2aec7ea0624298c8cc6f0bcb5f21b439f4e96304b8b47c8bf15ef8d`  
		Last Modified: Tue, 11 Oct 2022 20:35:04 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b45c9281c722e160d2675d4141a7174b59945582b16af0e76b2ff4b081b98ab9`  
		Last Modified: Wed, 12 Oct 2022 18:13:49 GMT  
		Size: 344.9 KB (344931 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dbe998af75050a5457d8dee24c1be38f71f8ef407b600c4f40b79d760bc46863`  
		Last Modified: Thu, 13 Oct 2022 23:26:11 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f15018699a72c3f947c845281bb9c038666d65548171b0549a2907a031da882`  
		Last Modified: Thu, 13 Oct 2022 23:26:14 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:09131b2774bcdb3d5d0937fe0b4acdbc40fc7f0553ea2f75e323487a0c957739`  
		Last Modified: Thu, 13 Oct 2022 23:26:21 GMT  
		Size: 54.4 MB (54434888 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
