| Elastic Premium | Flex |
| -- | -- |
|  [![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fmacavall%2Ftestflex5601%2Frefs%2Fheads%2Fmaster%2Ftemplate10.json) | [![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fmacavall%2Ftestflex5601%2Frefs%2Fheads%2Fmaster%2Fpefunc-flex.json) |

 Flex [![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fmacavall%2Ftestflex5601%2Frefs%2Fheads%2Fmaster%2FS1FuncMcp.json)

 Standard Linux [![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fmacavall%2Ftestflex5601%2Frefs%2Fheads%2Fmaster%2FS1funcmpc2.json)

 Bad Standard Linux [![Deploy to Azure](https://aka.ms/deploytoazurebutton)](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fmacavall%2Ftestflex5601%2Frefs%2Fheads%2Fmaster%2FS1LinuxFuncMpc.json)

[Elastic Premium deploy VNet Managed Identity with Key Vault](https://portal.azure.com/#create/Microsoft.Template/uri/https%3A%2F%2Fraw.githubusercontent.com%2Fmacavall%2Ftestflex5601%2Frefs%2Fheads%2Fmaster%2Felasticvnetman5.json)

```plain
dotnet publish -c Release -o .\bin\publish

Compress-Archive -Path .\bin\publish\* -DestinationPath ..\func_publish.zip -Force

az functionapp deployment source config-zip -g tester55 -n <APP_NAME> --src ..\func_publish.zip
```
