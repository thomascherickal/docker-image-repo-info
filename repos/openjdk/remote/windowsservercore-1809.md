## `openjdk:windowsservercore-1809`

```console
$ docker pull openjdk@sha256:17bf309bbcd729dbbf2c8f2cd9ca8846e0118ea59ebc28b0fc58eb9cc5496972
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.2114; amd64

### `openjdk:windowsservercore-1809` - windows version 10.0.17763.2114; amd64

```console
$ docker pull openjdk@sha256:2a989760f907d06b557aa1677dd06ec88f1b634163ca747200137d0f31830a8e
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.9 GB (2867115793 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:31d254172ca24271f48c57ef857c5b46d6b6435b50ac461b3e5838a97a971aa3`
-	Default Command: `["jshell"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Thu, 07 May 2020 05:09:25 GMT
RUN Apply image 1809-RTM-amd64
# Thu, 05 Aug 2021 19:44:34 GMT
RUN Install update 1809-amd64
# Wed, 11 Aug 2021 12:16:25 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 17:21:43 GMT
RUN Write-Host 'Enabling TLS 1.2 (https://githubengineering.com/crypto-removal-notice/) ...'; 	$tls12RegBase = 'HKLM:\\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2'; 	if (Test-Path $tls12RegBase) { throw ('"{0}" already exists!' -f $tls12RegBase) }; 	New-Item -Path ('{0}/Client' -f $tls12RegBase) -Force; 	New-Item -Path ('{0}/Server' -f $tls12RegBase) -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Client' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'DisabledByDefault' -PropertyType DWORD -Value 0 -Force; 	New-ItemProperty -Path ('{0}/Server' -f $tls12RegBase) -Name 'Enabled' -PropertyType DWORD -Value 1 -Force; 	Write-Host 'Complete.'
# Wed, 11 Aug 2021 17:40:45 GMT
ENV JAVA_HOME=C:\openjdk-16
# Wed, 11 Aug 2021 17:41:58 GMT
RUN $newPath = ('{0}\bin;{1}' -f $env:JAVA_HOME, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	setx /M PATH $newPath; 	Write-Host 'Complete.'
# Wed, 11 Aug 2021 17:42:02 GMT
ENV JAVA_VERSION=16.0.2
# Wed, 11 Aug 2021 17:42:05 GMT
ENV JAVA_URL=https://download.java.net/java/GA/jdk16.0.2/d4a915d82b4c4fbb9bde534da945d746/7/GPL/openjdk-16.0.2_windows-x64_bin.zip
# Wed, 11 Aug 2021 17:42:08 GMT
ENV JAVA_SHA256=9df98be05fe674066cc39144467c47b1503cfa3de059c09cc4ccc3da9c253b9a
# Wed, 11 Aug 2021 17:43:45 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:JAVA_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:JAVA_URL -OutFile 'openjdk.zip'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:JAVA_SHA256); 	if ((Get-FileHash openjdk.zip -Algorithm sha256).Hash -ne $env:JAVA_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	New-Item -ItemType Directory -Path C:\temp | Out-Null; 	Expand-Archive openjdk.zip -DestinationPath C:\temp; 	Move-Item -Path C:\temp\* -Destination $env:JAVA_HOME; 	Remove-Item C:\temp; 		Write-Host 'Removing ...'; 	Remove-Item openjdk.zip -Force; 		Write-Host 'Verifying install ...'; 	Write-Host '  javac --version'; javac --version; 	Write-Host '  java --version'; java --version; 		Write-Host 'Complete.'
# Wed, 11 Aug 2021 17:43:48 GMT
CMD ["jshell"]
```

-	Layers:
	-	`sha256:4612f6d0b889cad0ed0292fae3a0b0c8a9e49aff6dea8eb049b2386d9b07986f`  
		Size: 1.7 GB (1718332879 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c67ded6868b61d392a0c096f911563fd6bc0bc3ed4fe401d077b3718a1b0cdaf`  
		Size: 967.7 MB (967665054 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:f5be68d5dab08a1dcc52a6ee52dd4901e4d6a384f0df3a12cba3d53649f7c602`  
		Last Modified: Wed, 11 Aug 2021 13:29:37 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a93339de9664b8795350d24edfc9da5614b2c1711961e94e1cb0ca7cf7fae74a`  
		Last Modified: Wed, 11 Aug 2021 18:16:44 GMT  
		Size: 360.5 KB (360455 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2ae4ab29ae94349772a609651047824849543815a7e666afb0c7054d8ed260bc`  
		Last Modified: Wed, 11 Aug 2021 18:26:45 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:57b75111bdf3015fbfd015e869aa79f9c04f5a18a0299ecabc95e10494c985c9`  
		Last Modified: Wed, 11 Aug 2021 18:26:45 GMT  
		Size: 317.9 KB (317892 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:680002cb7bea099ff420cfd09908dd2c96dff1f4f1a280337829a50b601735e6`  
		Last Modified: Wed, 11 Aug 2021 18:26:42 GMT  
		Size: 1.4 KB (1402 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:775632d09d44fa82311e0f02768e548d26661886be204f5d0b5d6b54562032a6`  
		Last Modified: Wed, 11 Aug 2021 18:26:42 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:694e7d2ddf0129dcbd28683364aacd6918b30a5fbd6e04fccb0a2d5c99d7f05f`  
		Last Modified: Wed, 11 Aug 2021 18:26:42 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3b5a9bb34835e0fd2eacb32212556d4264509550109bf9c9bcb7484c20849356`  
		Last Modified: Wed, 11 Aug 2021 18:27:02 GMT  
		Size: 180.4 MB (180430973 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9e37577d4c666745bdd3d66b39247c3d71110fc04db964ca18afbc320806489e`  
		Last Modified: Wed, 11 Aug 2021 18:26:42 GMT  
		Size: 1.4 KB (1437 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
