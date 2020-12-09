## `adoptopenjdk:11-openj9-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:24f42dbf6af4fc44bdf36a3da1cf59a1568a76d09775ea69f6cd3aca640002f1
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4104; amd64

### `adoptopenjdk:11-openj9-windowsservercore-ltsc2016` - windows version 10.0.14393.4104; amd64

```console
$ docker pull adoptopenjdk@sha256:ee704246ae05ce577735a2755e4884bce9fd870912c10a10c151bb36b2eee29d
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.1 GB (6148957290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:c5a0f6a10efda34b71b4eb7707e7b22ded9de705136a24f628315481415e8af7`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 02 Dec 2020 17:42:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 09 Dec 2020 13:34:44 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 09 Dec 2020 21:12:08 GMT
ENV JAVA_VERSION=jdk-11.0.9+11_openj9-0.23.0
# Wed, 09 Dec 2020 21:16:33 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.9_11_openj9-0.23.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk11-binaries/releases/download/jdk-11.0.9%2B11_openj9-0.23.0/OpenJDK11U-jdk_x64_windows_openj9_11.0.9_11_openj9-0.23.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (c4885100b0565a63dc3e21a47c6e344ea863ec533d67664e06494385c5923cb3) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne 'c4885100b0565a63dc3e21a47c6e344ea863ec533d67664e06494385c5923cb3') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 09 Dec 2020 21:16:34 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 09 Dec 2020 21:16:35 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:d2696dc2a40dc121fc5acaa02242817ac416c69d17c113e2ac5136d21a3942d8`  
		Size: 1.7 GB (1698858125 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c6d005eb9e78ad42f77f3dad7e29d954e78f0547f9884fe024a71f4042412970`  
		Last Modified: Wed, 09 Dec 2020 13:55:31 GMT  
		Size: 1.2 KB (1186 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d453f78974223bb1f7e008edf5db3fe8d6e029ef3c5c833744353bf4e56aa67a`  
		Last Modified: Wed, 09 Dec 2020 22:08:11 GMT  
		Size: 1.1 KB (1127 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b805d9b4ea89943cc867c774b0d5336056499a4acc1c0d02fec900a6f8fc820`  
		Last Modified: Wed, 09 Dec 2020 22:08:41 GMT  
		Size: 380.1 MB (380108699 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0ce3251d98eb7e35d1abaa8794af242071b1b58c3d116b001802a1154dfa0cf1`  
		Last Modified: Wed, 09 Dec 2020 22:08:12 GMT  
		Size: 1.1 KB (1130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:ea60d7437dd421f9d0c61704bf049e8cc3267d63f920fd4ea96fe5991550351f`  
		Last Modified: Wed, 09 Dec 2020 22:08:11 GMT  
		Size: 1.1 KB (1123 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
