## `adoptopenjdk:11-hotspot-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:e48a09a20c8f0acd94a4b727234e6e79833bdc7233080b13b7a84d6efd26134c
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4283; amd64

### `adoptopenjdk:11-hotspot-windowsservercore-ltsc2016` - windows version 10.0.14393.4283; amd64

```console
$ docker pull adoptopenjdk@sha256:74eeea161df6e20b80209a6b81bf90c61fc8ddb42c900becadceccecf4edda82
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6170793842 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:efe1c3b2d737a1f52878da83aa93edab38347e846d3512f6947277a5dbab68eb`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 03 Mar 2021 18:02:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 10 Mar 2021 13:42:05 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 10 Mar 2021 19:18:19 GMT
ENV JAVA_VERSION=jdk-11.0.10+9
# Wed, 10 Mar 2021 19:22:52 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.10_9.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.10%2B9/OpenJDK11U-jdk_x64_windows_hotspot_11.0.10_9.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (f12011de94a72e1f14c9e68ce63bdd537aab1bf51eb336eba6d6061bc307baeb) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'f12011de94a72e1f14c9e68ce63bdd537aab1bf51eb336eba6d6061bc307baeb') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 10 Mar 2021 19:22:54 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:30bda99601c5cbd3b2118409f401852ea648e2319bd81518723e476b28d764c5`  
		Size: 1.7 GB (1726924885 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:76680da9dc6db108ddf2e353c494b45e8486a6751619a13ed8fb3ad64b9a16e9`  
		Last Modified: Wed, 10 Mar 2021 14:06:08 GMT  
		Size: 1.3 KB (1333 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f636df8bd7077554c6e3f64570497178fe86de606b0a6f88b777c476591c7586`  
		Last Modified: Wed, 10 Mar 2021 20:35:08 GMT  
		Size: 1.4 KB (1438 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ba2aef78c21ac76b94a6ea5195c54af2b6603f64c38732aa0926367a983d968`  
		Last Modified: Wed, 10 Mar 2021 20:35:42 GMT  
		Size: 373.9 MB (373878849 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b20402d5d086d5385b57dbd867b9eed12dd9fb24e530021e60f0b04b404374bc`  
		Last Modified: Wed, 10 Mar 2021 20:35:08 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
