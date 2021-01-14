## `adoptopenjdk:15-openj9-windowsservercore-ltsc2016`

```console
$ docker pull adoptopenjdk@sha256:5216db16aba10ca29d662d657da1a5e720a7f19018e9fcfef7b75590a4cea420
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4169; amd64

### `adoptopenjdk:15-openj9-windowsservercore-ltsc2016` - windows version 10.0.14393.4169; amd64

```console
$ docker pull adoptopenjdk@sha256:c1090cebb5c6f2e3120642eb9c38db1fd21089c5443e8036ca943d34ba04af8c
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.2 GB (6176760281 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:65d50194f969d307d306b6bdbda3ed54e6d70ff822011b7c65483d2752005d32`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Thu, 07 Jan 2021 11:30:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Jan 2021 13:37:06 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Jan 2021 22:56:59 GMT
ENV JAVA_VERSION=jdk-15.0.1+9_openj9-0.23.0
# Wed, 13 Jan 2021 23:00:12 GMT
RUN Write-Host ('Downloading https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9_openj9-0.23.0/OpenJDK15U-jdk_x64_windows_openj9_15.0.1_9_openj9-0.23.0.msi ...');     [Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12;     wget https://github.com/AdoptOpenJDK/openjdk15-binaries/releases/download/jdk-15.0.1%2B9_openj9-0.23.0/OpenJDK15U-jdk_x64_windows_openj9_15.0.1_9_openj9-0.23.0.msi -O 'openjdk.msi';     Write-Host ('Verifying sha256 (6745ab134f86bdb27154800fd0164a6d957c31a78a2cd812234d3c25639b0bf9) ...');     if ((Get-FileHash openjdk.msi -Algorithm sha256).Hash -ne '6745ab134f86bdb27154800fd0164a6d957c31a78a2cd812234d3c25639b0bf9') {             Write-Host 'FAILED!';             exit 1;     };         New-Item -ItemType Directory -Path C:\temp | Out-Null;         Write-Host 'Installing using MSI ...';     Start-Process -FilePath "msiexec.exe" -ArgumentList '/i', 'openjdk.msi', '/L*V', 'C:\temp\OpenJDK.log',     '/quiet', 'ADDLOCAL=FeatureEnvironment,FeatureJarFileRunWith,FeatureJavaHome' -Wait -Passthru;     Remove-Item -Path C:\temp -Recurse | Out-Null;     Write-Host 'Removing openjdk.msi ...';     Remove-Item openjdk.msi -Force
# Wed, 13 Jan 2021 23:00:13 GMT
ENV JAVA_TOOL_OPTIONS=-XX:+IgnoreUnrecognizedVMOptions -XX:+IdleTuningGcOnIdle
# Wed, 13 Jan 2021 23:00:14 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bd091f41e44cabc11504b7e130c74a7ef654f58840ba102e3507c4fdf2bae994`  
		Size: 1.7 GB (1723908142 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:51e9c5c519fdcd28aa0ed033a3cc16cf37dd76bea8ec06b2dc4a344415bdd224`  
		Last Modified: Wed, 13 Jan 2021 15:10:27 GMT  
		Size: 1.2 KB (1164 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b4134060a756ee99dc0ef9ef6ebfbb073550cfe0080607a4f33335dabe2b46fa`  
		Last Modified: Wed, 13 Jan 2021 23:45:55 GMT  
		Size: 1.1 KB (1147 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:43022f12d4e9bdba925b27c06af83bf0198569257a66efc59922c63cda68e37b`  
		Last Modified: Wed, 13 Jan 2021 23:46:25 GMT  
		Size: 382.9 MB (382861608 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:927e248e92b4becd9bebd24d41edffa44a4f8ff867acb8df195b5e196f8ca10f`  
		Last Modified: Wed, 13 Jan 2021 23:45:55 GMT  
		Size: 1.1 KB (1149 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b1716433a2f88747070d9854026b99baf599564154b28cda3d9cd7f72d86f65`  
		Last Modified: Wed, 13 Jan 2021 23:45:55 GMT  
		Size: 1.2 KB (1171 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
