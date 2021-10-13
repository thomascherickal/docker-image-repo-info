## `python:3-windowsservercore-ltsc2022`

```console
$ docker pull python@sha256:b70f1291fd72788bf4705da7a455fc9e7991030e28293b2da87d1aed2390825f
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.20348.288; amd64

### `python:3-windowsservercore-ltsc2022` - windows version 10.0.20348.288; amd64

```console
$ docker pull python@sha256:0e7f850929829cc5a4641dc046e70cead618e083e9ce0ad5ce80eb0acde44b61
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.2 GB (2195440534 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:792fc41f1d775893cd6b737d6d2a9ec374e0924238ae20665b0ac622f5a941b1`
-	Default Command: `["python"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Sat, 08 May 2021 09:40:24 GMT
RUN Apply image 2022-RTM-amd64
# Thu, 07 Oct 2021 11:33:56 GMT
RUN Install update ltsc2022-amd64
# Wed, 13 Oct 2021 12:26:42 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 13 Oct 2021 17:26:56 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 13 Oct 2021 17:34:07 GMT
ENV PYTHON_VERSION=3.10.0
# Wed, 13 Oct 2021 17:34:08 GMT
ENV PYTHON_RELEASE=3.10.0
# Wed, 13 Oct 2021 17:35:40 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f $env:PYTHON_RELEASE, $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 13 Oct 2021 17:35:41 GMT
ENV PYTHON_PIP_VERSION=21.2.4
# Wed, 13 Oct 2021 17:35:42 GMT
ENV PYTHON_SETUPTOOLS_VERSION=57.5.0
# Wed, 13 Oct 2021 17:35:44 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/d781367b97acf0ece7e9e304bf281e99b618bf10/public/get-pip.py
# Wed, 13 Oct 2021 17:35:45 GMT
ENV PYTHON_GET_PIP_SHA256=01249aa3e58ffb3e1686b7141b4e9aac4d398ef4ac3012ed9dff8dd9f685ffe0
# Wed, 13 Oct 2021 17:36:41 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 13 Oct 2021 17:36:42 GMT
CMD ["python"]
```

-	Layers:
	-	`sha256:8f616e6e9eec767c425fd9346648807d1b658d20ff6097be1d955aac69c26642`  
		Size: 1.3 GB (1251699055 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b03bbc71f9254a4ad2fba472595c859655b9d0cfefa638928416e277e0f0d497`  
		Size: 889.8 MB (889767519 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:b201e45e5b11128e36517715f5b6ae98e5782737c1b112a5fae2aa83206f57bf`  
		Last Modified: Wed, 13 Oct 2021 13:23:57 GMT  
		Size: 1.4 KB (1433 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:d98123f2c4ddfb33c96ba4a6bd915d08c855a3c8a662f0f5b6e166f2c7eb79bc`  
		Last Modified: Wed, 13 Oct 2021 17:57:32 GMT  
		Size: 1.4 KB (1379 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:53c80a20136695c56aa18eee8def72045d8098489264d68337d144bde31550e5`  
		Last Modified: Wed, 13 Oct 2021 17:58:13 GMT  
		Size: 1.4 KB (1357 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3d542ca50c9cebf987170089120d7709f0a868a8d6bda8225a2e547693486c70`  
		Last Modified: Wed, 13 Oct 2021 17:58:12 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:b6d38c807ba83039bf6c4fcf7caed86c78afe806244efb558faad3d45660cc5a`  
		Last Modified: Wed, 13 Oct 2021 17:59:05 GMT  
		Size: 47.3 MB (47259063 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:3f50a0470721cb491beb4b8019a0a4381cfdf8e618b8017f2e6c478a56487aaa`  
		Last Modified: Wed, 13 Oct 2021 17:58:12 GMT  
		Size: 1.4 KB (1415 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0dc997eb3054b13080196cdb0f82b2483ba32710b604acd43452dd6b43a9588f`  
		Last Modified: Wed, 13 Oct 2021 17:58:10 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:632aad4ff49e422c4d8d63983348076165c9cf766dc8ea2887f2f2d6fa0795b7`  
		Last Modified: Wed, 13 Oct 2021 17:58:10 GMT  
		Size: 1.4 KB (1387 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:defa69aa67dfdd6c8825394419817956c040aaa56ee18fb30f71b53c642c4100`  
		Last Modified: Wed, 13 Oct 2021 17:58:11 GMT  
		Size: 1.4 KB (1431 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:eef6054a81e49b006cf2179294e573220ed5578a3326c15945b697a0f7909ea7`  
		Last Modified: Wed, 13 Oct 2021 17:58:18 GMT  
		Size: 6.7 MB (6702225 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:0849a3b36bdd7ac7c73cd6f3059df634a56a9bedb67f8a0425fdc0329eadd4a7`  
		Last Modified: Wed, 13 Oct 2021 17:58:10 GMT  
		Size: 1.4 KB (1420 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
