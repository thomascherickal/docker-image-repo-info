## `hylang:python3.9-windowsservercore-ltsc2016`

```console
$ docker pull hylang@sha256:6ccccf3a101131a80600e3cf5523ae0375d9843df16f9e7b41e88b1b8b3371c9
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.14393.4583; amd64

### `hylang:python3.9-windowsservercore-ltsc2016` - windows version 10.0.14393.4583; amd64

```console
$ docker pull hylang@sha256:9e6f1813fb18c7a80534563cb752d0fa1acb6bbe1456904ebbcdd24dd6046e75
```

-	Docker Version: 20.10.7
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **6.3 GB (6332711710 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:d7e0d10fbb135bc9435bca412ea186e32adbf4a46a67812b647c0b10db448151`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 19 Nov 2016 17:05:00 GMT
RUN Apply image 1607-RTM-amd64
# Sun, 01 Aug 2021 08:52:00 GMT
RUN Install update ltsc2016-amd64
# Wed, 11 Aug 2021 12:51:34 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 11 Aug 2021 17:02:48 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 11 Aug 2021 17:12:15 GMT
ENV PYTHON_VERSION=3.9.6
# Wed, 11 Aug 2021 17:12:18 GMT
ENV PYTHON_RELEASE=3.9.6
# Wed, 11 Aug 2021 17:14:58 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Thu, 12 Aug 2021 20:20:54 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Thu, 12 Aug 2021 20:20:56 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/c20b0cfd643cd4a19246ccf204e2997af70f6b21/public/get-pip.py
# Thu, 12 Aug 2021 20:20:59 GMT
ENV PYTHON_GET_PIP_SHA256=fa6f3fb93cce234cd4e8dd2beb54a51ab9c247653b52855a48dd44e6b21ff28b
# Thu, 12 Aug 2021 20:23:01 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Thu, 12 Aug 2021 20:23:04 GMT
CMD ["python"]
# Thu, 12 Aug 2021 20:43:46 GMT
ENV HY_VERSION=1.0a3
# Thu, 12 Aug 2021 20:45:23 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION)
# Thu, 12 Aug 2021 20:45:25 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:3889bb8d808bbae6fa5a33e07093e65c31371bcf9e4c38c21be6b9af52ad1548`  
		Last Modified: Tue, 18 Sep 2018 20:20:50 GMT  
		Size: 4.1 GB (4069985900 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:c427f892fe74603ae09d4e49b25f8f7046f957054034dc9f462e0e88d7bffaa5`  
		Size: 2.2 GB (2200980134 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:2d4b5c087d85e7fbeffd8b282ecd862da1fb7ff00c37657c5712888936292097`  
		Last Modified: Wed, 11 Aug 2021 13:30:26 GMT  
		Size: 1.4 KB (1391 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:66b6dae97f6e4304e3285c8adf465d4e587122b9b3b548a8e5a1eda11a178c7d`  
		Last Modified: Wed, 11 Aug 2021 17:18:27 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:434173fe4dfb5d7cd14a0a85bfe806a956f75ccd348251558d53accaf212126d`  
		Last Modified: Wed, 11 Aug 2021 17:19:20 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:073b921580af3e47a105b3c2956f49113e4ce2cf379d65c1dab8d757126c4744`  
		Last Modified: Wed, 11 Aug 2021 17:19:20 GMT  
		Size: 1.4 KB (1430 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:6fd51408ca544dc1aa35e81c36b9acc94f5764c5e4260c7c442de747a95511cb`  
		Last Modified: Wed, 11 Aug 2021 17:19:28 GMT  
		Size: 54.1 MB (54145130 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2476bd0945dfce50571a71f22e7466f995cf472f151741f2ab717cd345f13579`  
		Last Modified: Thu, 12 Aug 2021 20:25:05 GMT  
		Size: 1.4 KB (1409 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:19ae605fa6a72bfeaab077778063d304d2fcc95d36a776333d49d819e1046354`  
		Last Modified: Thu, 12 Aug 2021 20:25:04 GMT  
		Size: 1.4 KB (1426 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f9d59e25a5e3fda4ba6fe87e5c0b036bd489db3132ee8043b55db9504599b746`  
		Last Modified: Thu, 12 Aug 2021 20:25:04 GMT  
		Size: 1.4 KB (1389 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9acaf3b9e038b75c7806e5231f61942d7b493126fbfcfb9d7b7442515d5cfd55`  
		Last Modified: Thu, 12 Aug 2021 20:25:08 GMT  
		Size: 6.3 MB (6288943 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:8b56115b80a461fee5b65fdc2009893290f036e1a554a8d947debc2bd98ba659`  
		Last Modified: Thu, 12 Aug 2021 20:25:04 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f7e3ac99b4211b8d3739f8447236b9f279c97a8f242f6a9869466b7a0e607267`  
		Last Modified: Thu, 12 Aug 2021 20:46:34 GMT  
		Size: 1.3 KB (1300 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:00a072b24fb55ca652471b3135a184f934940b6add13a13eb380adacf5a954b0`  
		Last Modified: Thu, 12 Aug 2021 20:46:34 GMT  
		Size: 1.3 MB (1297675 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5927788614ef25175e6c4edf7d2a1a1b3df0938f7303e547f0a473ef4d89b1dd`  
		Last Modified: Thu, 12 Aug 2021 20:46:34 GMT  
		Size: 1.3 KB (1305 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
