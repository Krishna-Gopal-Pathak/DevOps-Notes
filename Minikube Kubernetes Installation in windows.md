## Minikube Kubernetes Installation with chocolaty in windows

- Step 1- Install Oracle VM Virtualbox.
- Step 2- Run Powershell as administrator.
- Step 3- Below are Instructions to install chocolaty from Step 3 to Step 5. **OR** You can follow the official guide https://chocolatey.org/install

  **Note-** With PowerShell, you must ensure Get-ExecutionPolicy is not Restricted. We suggest using Bypass to bypass the policy to get things installed or AllSigned for quite a bit more security.

  Run **Get-ExecutionPolicy**. If it returns Restricted, then run **Set-ExecutionPolicy AllSigned** or **Set-ExecutionPolicy Bypass -Scope Process**.
  
  ```bash
  Get-ExecutionPolicy 
  ```
  ```bash
  Set-ExecutionPolicy AllSigned
  ```

- Step 4- Installing Chocolaty
  ```bash
  Set-ExecutionPolicy Bypass -Scope Process -Force; [System.Net.ServicePointManager]::SecurityProtocol = [System.Net.ServicePointManager]::SecurityProtocol -bor 3072; iex ((New-Object System.Net.WebClient).DownloadString('https://community.chocolatey.org/install.ps1'))
  ```
  **Note:** If getting Error, Turn Off Your Anti Virus for a moment and try again. Close powershell and start again

- Step 5- Check Choco version 
  ```bash
  choco --v
  ```
- Step 6- Restart Powershell as administrator.
- Step 7- Install Minikube with chocolaty
  ```bash
  choco install minikube kubernetes-cli -y
  ```
- Step 8- Check Minikube 
  ```bash
  minikube.exe --help
  ```
- Step 9- Execute to Setup Minikube cluster
  ```bash
  minikube start
  ```
