# az-cli

## Requirements

* az-cli
* jq
* xargs


```bash
az account subscription list \
  -o tsv \
  --query "[].{id: id, sub_id: subscriptionId, name: displayName}"

az costmanagement export list \
  --scope /subscriptions/x

az costmanagement export list \
  --scope "providers/Microsoft.Management/managementGroups/xx"

az billing invoice list

```
  --orderby time_asc \
  -o tsv \
  --query "[?lastUpdateTime < '2023-09-25'].[digest, lastUpdateTime]"

--query "[].{Size: imageSize, Tags: tags}" --output json > image_size.json
