## `openjdk:8u302-jre-windowsservercore-ltsc2016`

```console
$ docker pull openjdk@sha256:2e7aa908f9ffd79918d9cf19f976cf57d595c6f1ca84a9fb4074b60f14902157
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4704; amd64

### `openjdk:8u302-jre-windowsservercore-ltsc2016` - windows version 10.0.14393.4704; amd64

```console
$ docker pull openjdk@sha256:5e95e30812221ae959acf1196b0f339ab3b82d33a3d1674bf4cec0c5af140e32
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6312039108 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:b0524d3ae56a7babbeabe2c4c5801b96873ba1638b252bafdee24f1a4bd97e7e`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 06 Oct 2021 21:16:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 13 Oct 2021 12:40:35 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 14 Oct 2021 00:35:32 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Thu, 14 Oct 2021 01:06:30 GMT
ENV JAVA_HOME=C:\openjdk-8
# Thu, 14 Oct 2021 01:07:35 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Thu, 14 Oct 2021 01:07:36 GMT
ENV JAVA_VERSION=8u302
# Thu, 14 Oct 2021 01:11:32 GMT
ENV JAVA_URL=https://github.com/AdoptOpenJDK/openjdk8-upstream-binaries/releases/download/jdk8u302-b08/OpenJDK8U-jre_x64_windows_8u302b08.zip
# Thu, 14 Oct 2021 01:12:52 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  java -version'; java -version; 		Write-Host 'Complete.'
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:0c776a8e8e3c02d360995b7fa26a3fd7c0928965795fac57b69ff07418ab07bf`  
		Size: 2.2 GB (2202780626 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:6974b1bd85ba3f9ce16d86231eced43f720fed9c13411d37584dfe7193bcde60`  
		Last Modified: Wed, 13 Oct 2021 13:27:57 GMT  
		Size: 1.3 KB (1322 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0df06f60babff5e4f22bec0a3230e7cb06b975eee8a07f9541607a63c6f54ec1`  
		Last Modified: Sat, 16 Oct 2021 00:35:57 GMT  
		Size: 352.3 KB (352290 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:de0c4d3b2ec873e55c039f51a197f4de61458d4f05a18fbc82eeebe00b1b5886`  
		Last Modified: Sat, 16 Oct 2021 00:50:13 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1ea8b9c7731d764fa4e12975893be5abd39526f8ecc73b00ad2113009751e70c`  
		Last Modified: Sat, 16 Oct 2021 00:50:13 GMT  
		Size: 348.4 KB (348382 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c4ce1dccba2a2d699f13b831ecba8da857b410a935538aa72a3bf38bbe251f6`  
		Last Modified: Sat, 16 Oct 2021 00:50:13 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9cf32e9a46c96a9dceacc27a86efec66f50f97e76536df2c107414360539a6aa`  
		Last Modified: Sat, 16 Oct 2021 00:53:06 GMT  
		Size: 1.4 KB (1375 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:1c15710c1dfa3b56cfb23d30a34920c041f3b85519e20088ff0ef77b6bf623c3`  
		Last Modified: Sat, 16 Oct 2021 00:53:12 GMT  
		Size: 38.6 MB (38566351 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
