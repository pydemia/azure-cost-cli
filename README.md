# azure-cost-cli

See: https://github.com/mivano/azure-cost-cli

```bash
brew install dotnet

dotnet tool install --global azure-cost-cli 
dotnet tool update --global azure-cost-cli 

azure-cost --help
```

## Accumulated Cost

```bash
SUB_ID=574385a9-08e9-49fe-91a2-27660d92b8f5
azure-cost accumulatedCost -s $SUB_ID
```

## Cost by Tag

```bash
azure-cost costByTag  --tag cost-center --tag creator
```

