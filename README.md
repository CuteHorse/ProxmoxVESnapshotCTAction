example usage:

```
jobs:
  create-snapshot:
    needs: build-application
    uses:  "https://github.com/CuteHorse/ProxmoxVESnapshotCTAction/.github/workflows/CreateSnapshot.yml@master"
    with:
      domain: pve.example.com
      node-name: 'PVE'
      ct-id: '101'
      user: 'github@pve!tokenname'
    secrets:
      token: '00000000-0000-0000-0000-000000000000'
```
