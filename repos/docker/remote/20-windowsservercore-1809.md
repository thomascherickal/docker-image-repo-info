## `docker:20-windowsservercore-1809`

```console
$ docker pull docker@sha256:967a356e2301df83e5966c65a7443564af570a271d090739f0bed541e45b48c0
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3532; amd64

### `docker:20-windowsservercore-1809` - windows version 10.0.17763.3532; amd64

```console
$ docker pull docker@sha256:f86b72aa5f07d812867dc8d4e39a57a6701a82aeba5c1f0bf23c378f5f0529a1
```

-	Docker Version: 20.10.17
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.8 GB (2765941398 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:11422e900a3b4f74151ad09b19a129fc52b5bb295afa8648ef23703a1f1371ba`
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
# Wed, 12 Oct 2022 18:11:43 GMT
ENV DOCKER_VERSION=20.10.18
# Wed, 12 Oct 2022 18:11:43 GMT
ENV DOCKER_URL=https://download.docker.com/win/static/stable/x86_64/docker-20.10.18.zip
# Wed, 12 Oct 2022 18:13:03 GMT
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
	-	`sha256:484cb23406c81cee1317b6f4317cf91c90b2befbf286563417731d9625428a3d`  
		Last Modified: Wed, 12 Oct 2022 18:14:28 GMT  
		Size: 1.4 KB (1424 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d58fbdb2b2e396e552df91a674216265229b83e0849e3f52e61d570fb88cd6e3`  
		Last Modified: Wed, 12 Oct 2022 18:14:28 GMT  
		Size: 1.4 KB (1390 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85d8ddb2645a2f44e7e79b123dcd24e5ef377dc0dacb7a058beff26089fc9a67`  
		Last Modified: Wed, 12 Oct 2022 18:14:38 GMT  
		Size: 54.4 MB (54428286 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
