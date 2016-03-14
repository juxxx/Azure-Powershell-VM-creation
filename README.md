Azure-Powershell-VM-creation
Create a PowerShell script to remotely provision an Azure VM with Windows Sever 2012 Datacenter edition using the Azure PowerShell.

By default, script will need to be given the parameters 
- virtual machine name
- virtual machine size
- azure account subscription name

CreateAzureVM.ps1 -vmname "MyVMNameHere” -vmsize “MyVMSizeHere” -SubscriptionName “MySubsNameHere”

If some options needs to be modified, it's best done by changeing the corresponding variable values, defaults listed as follows:
$rgName = "vm_resource_group"

$locName = "North Europe"
$saName="testvmstorageaccount"
$saType="Standard_LRS"
$domName="new-test-vm-environment"
$vnetName="TestNet"
$nicName="vmNIC"
$pubName="MicrosoftWindowsServer"
$offerName="WindowsServer"
$skuName="2012-R2-Datacenter"
$diskName="OSDisk"

