## `hylang:python3.9-windowsservercore-1809`

```console
$ docker pull hylang@sha256:abf6a1368944608694777cc42bfd1e0f20dc79976ea80c0bcd579ca564a7afff
```

-	Manifest MIME: `application/vnd.docker.distribution.manifest.list.v2+json`
-	Platforms: 1
	-	windows version 10.0.17763.3046; amd64

### `hylang:python3.9-windowsservercore-1809` - windows version 10.0.17763.3046; amd64

```console
$ docker pull hylang@sha256:01df47e247cbcc15e8ba3189c9bb2715a1c93617b60c184df44c86785487c077
```

-	Docker Version: 20.10.8
-	Manifest MIME: `application/vnd.docker.distribution.manifest.v2+json`
-	Total Size: **2.7 GB (2722135133 bytes)**  
	(compressed transfer size, not on-disk size)
-	Image ID: `sha256:3821765f7a8142e6eabd294e47ccad3f3ac10470815e40cb7fd72d72b5ca6acd`
-	Default Command: `["hy"]`
-	`SHELL`: `["powershell","-Command","$ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';"]`

```dockerfile
# Fri, 22 Apr 2022 01:27:13 GMT
RUN Apply image 10.0.17763.2803
# Thu, 09 Jun 2022 19:41:03 GMT
RUN Install update 10.0.17763.3046
# Wed, 15 Jun 2022 12:18:31 GMT
SHELL [powershell -Command $ErrorActionPreference = 'Stop'; $ProgressPreference = 'SilentlyContinue';]
# Wed, 15 Jun 2022 12:41:47 GMT
ENV PYTHONIOENCODING=UTF-8
# Wed, 15 Jun 2022 17:16:28 GMT
ENV PYTHON_VERSION=3.9.13
# Wed, 15 Jun 2022 17:18:32 GMT
RUN $url = ('https://www.python.org/ftp/python/{0}/python-{1}-amd64.exe' -f ($env:PYTHON_VERSION -replace '[a-z]+[0-9]*$', ''), $env:PYTHON_VERSION); 	Write-Host ('Downloading {0} ...' -f $url); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $url -OutFile 'python.exe'; 		Write-Host 'Installing ...'; 	$exitCode = (Start-Process python.exe -Wait -NoNewWindow -PassThru 		-ArgumentList @( 			'/quiet', 			'InstallAllUsers=1', 			'TargetDir=C:\Python', 			'PrependPath=1', 			'Shortcuts=0', 			'Include_doc=0', 			'Include_pip=0', 			'Include_test=0' 		) 	).ExitCode; 	if ($exitCode -ne 0) { 		Write-Host ('Running python installer failed with exit code: {0}' -f $exitCode); 		Get-ChildItem $env:TEMP | Sort-Object -Descending -Property LastWriteTime | Select-Object -First 1 | Get-Content; 		exit $exitCode; 	} 		$env:PATH = [Environment]::GetEnvironmentVariable('PATH', [EnvironmentVariableTarget]::Machine); 		Write-Host 'Verifying install ...'; 	Write-Host '  python --version'; python --version; 		Write-Host 'Removing ...'; 	Remove-Item python.exe -Force; 	Remove-Item $env:TEMP/Python*.log -Force; 		Write-Host 'Complete.'
# Wed, 15 Jun 2022 17:18:36 GMT
ENV PYTHON_PIP_VERSION=22.0.4
# Wed, 15 Jun 2022 17:18:37 GMT
ENV PYTHON_SETUPTOOLS_VERSION=58.1.0
# Wed, 15 Jun 2022 17:18:38 GMT
ENV PYTHON_GET_PIP_URL=https://github.com/pypa/get-pip/raw/6ce3639da143c5d79b44f94b04080abf2531fd6e/public/get-pip.py
# Wed, 15 Jun 2022 17:18:39 GMT
ENV PYTHON_GET_PIP_SHA256=ba3ab8267d91fd41c58dbce08f76db99f747f716d85ce1865813842bb035524d
# Wed, 15 Jun 2022 17:20:20 GMT
RUN Write-Host ('Downloading get-pip.py ({0}) ...' -f $env:PYTHON_GET_PIP_URL); 	[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12; 	Invoke-WebRequest -Uri $env:PYTHON_GET_PIP_URL -OutFile 'get-pip.py'; 	Write-Host ('Verifying sha256 ({0}) ...' -f $env:PYTHON_GET_PIP_SHA256); 	if ((Get-FileHash 'get-pip.py' -Algorithm sha256).Hash -ne $env:PYTHON_GET_PIP_SHA256) { 		Write-Host 'FAILED!'; 		exit 1; 	}; 		$env:PYTHONDONTWRITEBYTECODE = '1'; 		Write-Host ('Installing pip=={0} ...' -f $env:PYTHON_PIP_VERSION); 	python get-pip.py 		--disable-pip-version-check 		--no-cache-dir 		--no-compile 		('pip=={0}' -f $env:PYTHON_PIP_VERSION) 		('setuptools=={0}' -f $env:PYTHON_SETUPTOOLS_VERSION) 	; 	Remove-Item get-pip.py -Force; 		Write-Host 'Verifying pip install ...'; 	pip --version; 		Write-Host 'Complete.'
# Wed, 15 Jun 2022 17:20:21 GMT
CMD ["python"]
# Wed, 15 Jun 2022 20:33:01 GMT
ENV HY_VERSION=1.0a4
# Wed, 15 Jun 2022 20:33:02 GMT
ENV HYRULE_VERSION=0.1
# Wed, 15 Jun 2022 20:34:23 GMT
RUN pip install --no-cache-dir ('hy == {0}' -f $env:HY_VERSION) ('hyrule == {0}' -f $env:HYRULE_VERSION)
# Wed, 15 Jun 2022 20:34:24 GMT
CMD ["hy"]
```

-	Layers:
	-	`sha256:b111c3320c949bea81612bf4554f1b6592c2f504920b5bf57ba340a1d4d52c93`  
		Size: 1.9 GB (1877166088 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:fc6ae6c5aa2b4920ae68469c5e7e7c3a3c85e5eaafc24660e7b3adb21d6fce77`  
		Size: 786.1 MB (786113785 bytes)  
		MIME: application/vnd.docker.image.rootfs.foreign.diff.tar.gzip
	-	`sha256:4ed911f97ae3a2a6279c70738e5692b14369ac11871a2bbd2f6ad301419527ad`  
		Last Modified: Wed, 15 Jun 2022 12:50:13 GMT  
		Size: 1.3 KB (1314 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:5a06c506fd1c86229974813982c21c141062b8d6df41c48831faa8ad1fd29cff`  
		Last Modified: Wed, 15 Jun 2022 12:54:55 GMT  
		Size: 1.3 KB (1313 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fdf08e1caa749f366733e7b1d4b6503cf4f7771fdb79a22f8e5f0458d806975a`  
		Last Modified: Wed, 15 Jun 2022 17:24:09 GMT  
		Size: 1.4 KB (1414 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:c2d6d3489ee50af2384b59d5b323304c59b5e48b098999f9995e8f3a9ae6d16a`  
		Last Modified: Wed, 15 Jun 2022 17:25:03 GMT  
		Size: 51.7 MB (51712720 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:03ea059fe6fadcc69782d5ec7643b7a88a843a64e11e4a2cd263000cbe8856ef`  
		Last Modified: Wed, 15 Jun 2022 17:24:09 GMT  
		Size: 1.4 KB (1412 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:4e0930641185376d0d83d5f8e7fe0c86e007817c1e28e05c6a94bc70ed0b78c0`  
		Last Modified: Wed, 15 Jun 2022 17:24:07 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:91edb99c9443499cd793e3c9a37afae8dc3fce0cd8ca878e53f3ab3052b47eb8`  
		Last Modified: Wed, 15 Jun 2022 17:24:07 GMT  
		Size: 1.4 KB (1425 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:77b57194d07d328ec2fa341efcde835d2bc1d2582f1b5b2d6b3d7949b3f3e231`  
		Last Modified: Wed, 15 Jun 2022 17:24:07 GMT  
		Size: 1.4 KB (1416 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:fab3bc5b76cb87a2d533a1f4d7b4b2d858c9136ff38929af04c127d44425f201`  
		Last Modified: Wed, 15 Jun 2022 17:24:08 GMT  
		Size: 3.5 MB (3487643 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9742e1073b06ea3570e0fb9e8c941fe860bc66d3783f57e3f42d114be6cbc60b`  
		Last Modified: Wed, 15 Jun 2022 17:24:07 GMT  
		Size: 1.4 KB (1442 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:aac697823db6043784a81de1fb6239bbe0137630b827c7dbc588cab8677cf1db`  
		Last Modified: Wed, 15 Jun 2022 20:44:23 GMT  
		Size: 1.4 KB (1421 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:2b072c537f19feb2d4e032ed78775dbc8ed6e1e56d9baac01787402c19ebcb12`  
		Last Modified: Wed, 15 Jun 2022 20:44:23 GMT  
		Size: 1.4 KB (1419 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:f42b04611d8735007d253466e1b1bae45334008735904b0e0aa00b743d953200`  
		Last Modified: Wed, 15 Jun 2022 20:44:27 GMT  
		Size: 3.6 MB (3639483 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
	-	`sha256:9d37d2ccd4020722bde3839cb2ac43581794e095d3f2acd8bc7fa842ddab2d8b`  
		Last Modified: Wed, 15 Jun 2022 20:44:23 GMT  
		Size: 1.4 KB (1422 bytes)  
		MIME: application/vnd.docker.image.rootfs.diff.tar.gzip
