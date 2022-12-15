# actions-xcode-create-simulator

```yml
steps:
  - uses: muukii/actions-xcode-install-simulator@main
    with:
      ios_version: '13.7'
  - uses: muukii/actions-xcode-create-simulator@main
    id: target
    with:
      device: 'iPhone 8'
      runtime: '13.7
  - run: echo ${{ steps.target.outputs.uuid }}
```
