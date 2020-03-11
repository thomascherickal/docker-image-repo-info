## `golang:windowsservercore`

```console
$ docker pull golang@sha256:7820ad9ec05f130433ae87d063c0f1cfb5723dd04acc9f7a296fdd9fd52ecc1a
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.3506; amd64
	-	windows version 10.0.17763.1098; amd64

### `golang:windowsservercore` - windows version 10.0.14393.3506; amd64

```console
$ docker pull golang@sha256:70ee2e2309c511b95a695bf5abae98406dd72ed89c939e6e33a094049f0a8982
```

-	Docker Version: 18.03.1-ee-4
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5905555290 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:ee8b972741e20cc99b5edb55931c3665ec1b9a9a495c13e6015c6946afcedbbb`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Fri, 14 Feb 2020 21:42:00 GMT
RUN Install update ltsc2016-amd64
# Thu, 20 Feb 2020 01:48:27 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Thu, 20 Feb 2020 09:14:29 GMT
ENV GIT_VERSION=2.23.0
# Thu, 20 Feb 2020 09:14:30 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Thu, 20 Feb 2020 09:14:31 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Thu, 20 Feb 2020 09:14:33 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Thu, 20 Feb 2020 09:16:15 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Thu, 20 Feb 2020 09:16:17 GMT
ENV GOPATH=C:\gopath
# Thu, 20 Feb 2020 09:17:39 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 26 Feb 2020 00:24:17 GMT
ENV GOLANG_VERSION=1.14
# Wed, 26 Feb 2020 00:31:39 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'cc2f1e8d19744fe0b2e979bf9a4f9d224e416f4f54cb6cf3aa8b5e9c0865de37'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 26 Feb 2020 00:31:41 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:846a2223e9e7a88a2a07d706553f144d380483d72fb9f0697c4fcd71773a8693`  
		Size: 1.7 GB (1657079102 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:72c4471958f7f0f07260f0f430bcffb0bc07811088c24cffba1439d250ea1ae3`  
		Last Modified: Thu, 20 Feb 2020 03:04:52 GMT  
		Size: 1.2 KB (1181 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:560a5edc3b65548cd8f0a5736740259c10731b69be646647541d454f4a46d74d`  
		Last Modified: Thu, 20 Feb 2020 10:16:28 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d778cb1587245dbb3aa1eadff960d2ca6808181a7f76399e1461b4488dd0d110`  
		Last Modified: Thu, 20 Feb 2020 10:16:27 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7cc71d139522c2d69f799715a806ce8ce02bd536d9fb33c3c1cff0d512c06ebe`  
		Last Modified: Thu, 20 Feb 2020 10:16:25 GMT  
		Size: 1.2 KB (1184 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6c3aec6ae82f728acb67ab3203c9f84faf93c0ff671c1d1341837da6f6127ec3`  
		Last Modified: Thu, 20 Feb 2020 10:16:25 GMT  
		Size: 1.2 KB (1212 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6734e518b8f70059c148a428fbd47fe51d143e43477597a7b34afb502090a6cd`  
		Last Modified: Thu, 20 Feb 2020 10:16:57 GMT  
		Size: 30.5 MB (30460160 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a52c1cb26338697dbffd8fd282e956aa88db7f630a7b5c1c90f750eee04c24e4`  
		Last Modified: Thu, 20 Feb 2020 10:16:22 GMT  
		Size: 1.2 KB (1182 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:a58993efc965e34067a71381b74e269f61cff043dfd64a430cddfcd494cd3f21`  
		Last Modified: Thu, 20 Feb 2020 10:16:24 GMT  
		Size: 5.3 MB (5316014 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d7346524e3170cae52e12ecf555dfa52b9ccd9595caebb7bd8ad48d9573ea9e9`  
		Last Modified: Wed, 26 Feb 2020 00:45:02 GMT  
		Size: 1.2 KB (1213 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0f79df10c0d625a69d6eab9a3e306a15502d190b55ea12b3b74aad531144875c`  
		Last Modified: Wed, 26 Feb 2020 00:46:44 GMT  
		Size: 142.7 MB (142704440 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:dcad0e327f58fe14b1d910c5f02f0b0195f9b99ea4d1bc3b5702f65bfbbd9c31`  
		Last Modified: Wed, 26 Feb 2020 00:45:01 GMT  
		Size: 1.3 KB (1336 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip

### `golang:windowsservercore` - windows version 10.0.17763.1098; amd64

```console
$ docker pull golang@sha256:61b5512b182df40c79fa3039a08166173de2744e889f5022f21df9c80d337a9d
```

-	Docker Version: 18.09.11
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.4 GB (2428550568 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:035e0b16be1fd98c0bffadaa871d10ebe97d302d905d7c02593db406d69ae35b`
-	Default Command: `["c:\\windows\\system32\\cmd.exe"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 15 Sep 2018 09:10:26 GMT
RUN Apply image 1809-RTM-amd64
# Fri, 06 Mar 2020 11:12:29 GMT
RUN Install update 1809-amd64
# Wed, 11 Mar 2020 00:42:10 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Mar 2020 12:14:42 GMT
ENV GIT_VERSION=2.23.0
# Wed, 11 Mar 2020 12:14:44 GMT
ENV GIT_TAG=v2.23.0.windows.1
# Wed, 11 Mar 2020 12:14:46 GMT
ENV GIT_DOWNLOAD_URL=https://github.com/git-for-windows/git/releases/download/v2.23.0.windows.1/MinGit-2.23.0-64-bit.zip
# Wed, 11 Mar 2020 12:14:47 GMT
ENV GIT_DOWNLOAD_SHA256=8f65208f92c0b4c3ae4c0cf02d4b5f6791d539cd1a07b2df62b7116467724735
# Wed, 11 Mar 2020 12:15:54 GMT
RUN Write-Host ('Downloading {0} ...' -f $env:GIT_DOWNLOAD_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:GIT_DOWNLOAD_URL -OutFile 'git.zip'; 		Write-Host ('Verifying sha256 ({0}) ...' -f $env:GIT_DOWNLOAD_SHA256); 	if ((Get-FileHash git.zip -Algorithm sha256).Hash -ne $env:GIT_DOWNLOAD_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive -Path git.zip -DestinationPath C:\git\.; 		Write-Host 'Removing ...'; 	Remove-Item git.zip -Force; 		Write-Host 'Updating PATH ...'; 	$env:PATH = 'C:\git\cmd;C:\git\mingw64\bin;C:\git\usr\bin;' + $env:PATH; 	[Environment]::SetEnvironmentVariable('PATH', $env:PATH, [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ("git version") ...'; 	git version; 		Write-Host 'Complete.';
# Wed, 11 Mar 2020 12:15:56 GMT
ENV GOPATH=C:\gopath
# Wed, 11 Mar 2020 12:16:23 GMT
RUN $newPath = ('{0}\bin;C:\go\bin;{1}' -f $env:GOPATH, $env:PATH); 	Write-Host ('Updating PATH: {0}' -f $newPath); 	[Environment]::SetEnvironmentVariable('PATH', $newPath, [EnvironmentVariableTarget]::Machine);
# Wed, 11 Mar 2020 12:16:24 GMT
ENV GOLANG_VERSION=1.14
# Wed, 11 Mar 2020 12:22:26 GMT
RUN $url = ('https://golang.org/dl/go{0}.windows-amd64.zip' -f $env:GOLANG_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	Invoke-WebRequest -Uri $url -OutFile 'go.zip'; 		$sha256 = 'cc2f1e8d19744fe0b2e979bf9a4f9d224e416f4f54cb6cf3aa8b5e9c0865de37'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $sha256); 	if ((Get-FileHash go.zip -Algorithm sha256).Hash -ne $sha256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host 'Expanding ...'; 	Expand-Archive go.zip -DestinationPath C:\; 		Write-Host 'Removing ...'; 	Remove-Item go.zip -Force; 		Write-Host 'Verifying install ("go version") ...'; 	go version; 		Write-Host 'Complete.';
# Wed, 11 Mar 2020 12:22:29 GMT
WORKDIR C:\gopath
```

-	Layers:
	-	`sha256:65014b3c312172f10bd6701a063f9b5aaf9a916c2d2cb843d406a6f77ded3f8d`  
		Last Modified: Tue, 13 Nov 2018 18:50:17 GMT  
		Size: 1.5 GB (1534685324 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:23645bd7ee0885911e1e2ab55ebcb36ce35795e1ceba9166ffd1b26dde18c3ee`  
		Size: 730.7 MB (730650958 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:a7fab05ac5ad4b2f665ad71b5c08a81e82bff7ea2fdcbb66c14193d2dd268875`  
		Last Modified: Wed, 11 Mar 2020 01:16:21 GMT  
		Size: 1.2 KB (1210 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:faa59504e8a6021f126b043b84b365caa6366766b8fb31f9152e0f859bcfe743`  
		Last Modified: Wed, 11 Mar 2020 12:42:15 GMT  
		Size: 1.2 KB (1192 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66e8d18d31c69c104e81cb83056a05bf2d4e6d4c9c834cd23a1dd372bf5eba4b`  
		Last Modified: Wed, 11 Mar 2020 12:42:05 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8bc519099bf17d9b046eef0d0e32d954dc7e54a0fa76708db3ae859a8c63b5e2`  
		Last Modified: Wed, 11 Mar 2020 12:42:04 GMT  
		Size: 1.2 KB (1217 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:97ea92b91b1802207727bccdc5c099ba74e7557140d361b762c6107aa11d4632`  
		Last Modified: Wed, 11 Mar 2020 12:42:03 GMT  
		Size: 1.2 KB (1218 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:314fd97d425237bbcc41f14758f52ad3fde96f2c80c5eccb26754caf0c6648ad`  
		Last Modified: Wed, 11 Mar 2020 12:42:32 GMT  
		Size: 29.8 MB (29750573 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8237be75b55557e43ddf8cbe4cb67c918a149b9c971ec24857c862665f51ff34`  
		Last Modified: Wed, 11 Mar 2020 12:41:56 GMT  
		Size: 1.2 KB (1216 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5cf58a99dd488ee114fd242abf7b0cd3467bd9fba336c94c09c57f5f98355bad`  
		Last Modified: Wed, 11 Mar 2020 12:41:56 GMT  
		Size: 293.4 KB (293392 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c659989f91fcd5167e2630a8bed5ef54e13f9357608b8b9697bdc3900ef4ba1b`  
		Last Modified: Wed, 11 Mar 2020 12:41:56 GMT  
		Size: 1.2 KB (1191 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:af18bac2a8d8321bc8b9765ba7d77b520c4a0e205fef5b1c8488a8fd408e7974`  
		Last Modified: Wed, 11 Mar 2020 12:44:03 GMT  
		Size: 133.2 MB (133160510 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:85e4d6e9a77dc9cfe3a5247c21a283ca3eb19ee47ffdccbf26762096baf1faef`  
		Last Modified: Wed, 11 Mar 2020 12:41:56 GMT  
		Size: 1.3 KB (1349 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
