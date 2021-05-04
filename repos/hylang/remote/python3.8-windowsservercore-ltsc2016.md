## `hylang:python3.8-windowsservercore-ltsc2016`

```console
$ docker pull hylang@sha256:bd1971ffe0bd9c0bbc5b6954b194d99bd8f68f7ffb23e8b2750b8f151fec0f0b
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms:
	-	windows version 10.0.14393.4350; amd64

### `hylang:python3.8-windowsservercore-ltsc2016` - windows version 10.0.14393.4350; amd64

```console
$ docker pull hylang@sha256:57d507760d94820839402fba599d0af915fdedcf0dba8878bdae9083f20bbbef
```

-	Docker Version: 19.03.5
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **5.9 GB (5871428469 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:1d56e7417328e4def28b716f7a46cc31ea62202ce5ed1d568f8e05bdda339ac1`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Wed, 07 Apr 2021 21:54:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 14 Apr 2021 12:35:33 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 14 Apr 2021 16:15:18 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 14 Apr 2021 16:32:16 GMT
ENV PYTHON_VERSION=3.8.9
# Wed, 14 Apr 2021 16:32:17 GMT
ENV PYTHON_RELEASE=3.8.9
# Wed, 14 Apr 2021 16:34:56 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Mon, 03 May 2021 21:22:44 GMT
ENV PYTHON_PIP_VERSION=21.1.1
# Mon, 03 May 2021 21:22:45 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/1954f15b3f102ace496a34a013ea76b061535bd2/public/get-pip.py
# Mon, 03 May 2021 21:22:46 GMT
ENV PYTHON_GET_PIP_SHA256=f499d76e0149a673fb8246d88e116db589afbd291739bd84f2cd9a7bca7b6993
# Mon, 03 May 2021 21:24:29 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Mon, 03 May 2021 21:24:30 GMT
CMD ["python"]
# Mon, 03 May 2021 21:47:16 GMT
ENV HY_VERSION=1.0a1
# Mon, 03 May 2021 21:48:51 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Mon, 03 May 2021 21:48:52 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:00b4edb823e6a375d179a28cbfa682c2379d62179e1518485902d6e68b9a9d1e`  
		Size: 1.7 GB (1724897968 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:bb52885e05952959b0fa7aaff23561fcf14d294aed336112b388c94e67709e4f`  
		Last Modified: Wed, 14 Apr 2021 12:59:14 GMT  
		Size: 1.4 KB (1406 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:32b4598ab88dab64b25b4257872564af9825cc6cd41fc8cc1ad11c32958d0da9`  
		Last Modified: Wed, 14 Apr 2021 16:39:38 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8e2ba2f82f3eddbacdc29cc778a55d06ae05a67ecde117b71217e52591dab5f2`  
		Last Modified: Wed, 14 Apr 2021 16:42:34 GMT  
		Size: 1.4 KB (1427 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5e9327741bb35a9e94c5d9774ebf204c6256a8f84fa6fa63112bcb14e5fb3580`  
		Last Modified: Wed, 14 Apr 2021 16:42:34 GMT  
		Size: 1.4 KB (1403 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b761757c76a5489a33afa548887814f66f6d6414128957a48a9511cb178d1109`  
		Last Modified: Wed, 14 Apr 2021 16:42:44 GMT  
		Size: 58.6 MB (58623548 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:70a82d1f4fd0ba4c90790db5f76c74b35848dca224f36e092872dc46790eb1cf`  
		Last Modified: Mon, 03 May 2021 21:26:53 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:baf0ae193b42a8e89f98660ecb223e29c98e269d644057a9f11820d880d6fdcb`  
		Last Modified: Mon, 03 May 2021 21:26:53 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8f021fee546af25ca0fa91b58058abe8abc9b0c87884435767118ee5b1a83774`  
		Last Modified: Mon, 03 May 2021 21:26:53 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:79f13b4391bba40f58c57ce9403139bb7028cb7fbb21870c62e8936b0af702e7`  
		Last Modified: Mon, 03 May 2021 21:26:57 GMT  
		Size: 11.4 MB (11445694 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:cd47d94cbc6d6f0526eedcf12918458616c43fbc8562a0622781b1f29fda9047`  
		Last Modified: Mon, 03 May 2021 21:26:53 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:7d6f6b180e54d98ee1a48e3f2493ce654f3c54ee24935af1e93f6b21e7f58a7d`  
		Last Modified: Mon, 03 May 2021 21:53:07 GMT  
		Size: 1.4 KB (1405 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b74a611ec024d9b538e85e666054fcc40dd405605e7937420a1ec1683fbcebb3`  
		Last Modified: Mon, 03 May 2021 21:53:15 GMT  
		Size: 6.5 MB (6461359 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:28434547553679265f0c89a0b9d660f8d9cb3040d5503d3dd5da6223af4293e5`  
		Last Modified: Mon, 03 May 2021 21:53:07 GMT  
		Size: 1.3 KB (1329 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
