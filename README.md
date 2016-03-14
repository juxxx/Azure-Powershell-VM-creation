Azure-Powershell-VM-creation
Create a PowerShell script to remotely provision an Azure VM with Windows Sever 2012 Datacenter edition using the Azure PowerShell.

By default, script will need to be given the parameters 
- virtual machine name
- virtual machine size
- virtual machine NIC name
- azure account subscription name

CreateAzureVM.ps1 -vmname "MyVMNameHere” -vmsize “MyVMSizeHere” -nicName "MyNICNameHere" -subscr “MySubsNameHere” 

If some options needs to be modified, it's best done by changing the corresponding variable values, defaults listed as follows:

# $subscr = "Free_Trial"
# $vmName="TestVm_X"
# $vmSize="Standard_A1"
# $nicName="vmNIC"
$rgName = "vm_resource_group"
$locName = "North Europe"
$saName="jukkatpmvmstorage"
$saType="Standard_LRS"
$vnetName="TestNet"
$subnetIndex=0
$pubName="MicrosoftWindowsServer"
$offerName="WindowsServer"
$skuName="2012-R2-Datacenter"
$diskName="OSDisk"
