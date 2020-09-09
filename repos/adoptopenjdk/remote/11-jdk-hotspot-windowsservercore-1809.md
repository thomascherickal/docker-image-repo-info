## `adoptopenjdk:11-jdk-hotspot-windowsservercore-1809`

```console
$ docker pull adoptopenjdk@sha256:fd13c0f2454463990aa0cc7939d91de7485c59827f9cc6ee13cb71bdb8e1e02f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.17763.1457; amd64

### `adoptopenjdk:11-jdk-hotspot-windowsservercore-1809` - windows version 10.0.17763.1457; amd64

```console
$ docker pull adoptopenjdk@sha256:1e3fc9703bc1a8bfaa7f2fe7a311f9b8438696eadb66ba69930485c7e898cdfa
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2720838363 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:f0163d2aeeac125f4625fb62178dace5a6ae3f2956767f7cd0db1eba53a5ef0e`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 03 Sep 2020 05:59:01 GMT
RUN Install update 1809-amd64
# Tue, 08 Sep 2020 19:36:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Sep 2020 18:04:46 GMT
ENV JAVA_VERSION=jdk-11.0.8+10
# Wed, 09 Sep 2020 18:07:10 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jdk_x64_windows_hotspot_11.0.8_10.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.8%2B10/OpenJDK11U-jdk_x64_windows_hotspot_11.0.8_10.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (148b487e0dde39ec5c0f32aa2397c17968b6cf6818822cea2b2394dfd0157396) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '148b487e0dde39ec5c0f32aa2397c17968b6cf6818822cea2b2394dfd0157396') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Sep 2020 18:07:11 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c3aff44502467b94164764856a6feb805fc5c79ff66012eebdd7da3f180e3138`  
		Size: 632.9 MB (632939341 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:5af76ffebd6bf4f1b787b4a988842077427c65d101c4e4c449f02b8cea0332cd`  
		Last Modified: Tue, 08 Sep 2020 19:54:19 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:e9a273647a9d5ad5f2ad6d1d2c8fa6d8613de66e210fd2274f7822dd6555b29f`  
		Last Modified: Wed, 09 Sep 2020 19:15:49 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4553933d3d95c542e83b15c2676ceda32e5716645ec6b4d8f6cc9b5ac25ddba7`  
		Last Modified: Wed, 09 Sep 2020 19:16:29 GMT  
		Size: 369.6 MB (369562672 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b134ae8569651e16af12c9814451cbe28515f930a3824287d9b7ad42c134c043`  
		Last Modified: Wed, 09 Sep 2020 19:15:50 GMT  
		Size: 1.1 KB (1150 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
