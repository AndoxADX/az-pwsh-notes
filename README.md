# az-pwsh-notes
## useful powershell scripts for azure

# see version of powershell
$PsVersionTable

# install azure powershell module
Install-Module -Name Az -AllowClobber

# connect to azure accounts to login
Connect-AzAccount

# get list of subscriptions after logged in
Get-AzSubscription

# set the default
Select-AzSubscription -Subscription 'MySubscriptionName'

# see the current default subscription
Get-AzContext

PS>cd /mydir
PS>./myfile.ps1

# See the execution policy on your computer
Get-ExecutionPolicy -List

# Set the execution policy for the session. 
Set-ExecutionPolicy -Scope Process -ExecutionPolicy Bypass
