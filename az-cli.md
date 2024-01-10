# az-cli

```bash
az account subscription list
```
  --orderby time_asc \
  -o tsv \
  --query "[?lastUpdateTime < '2023-09-25'].[digest, lastUpdateTime]"

--query "[].{Size: imageSize, Tags: tags}" --output json > corus_image_size.json
