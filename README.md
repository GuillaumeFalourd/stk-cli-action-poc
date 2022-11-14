# stk-cli-action-poc

[![Action test Ubuntu](https://github.com/GuillaumeFalourd/stk-cli-action-poc/actions/workflows/action-test-ubuntu.yml/badge.svg)](https://github.com/GuillaumeFalourd/stk-cli-action-poc/actions/workflows/action-test-ubuntu.yml) [![Action test MacOS](https://github.com/GuillaumeFalourd/stk-cli-action-poc/actions/workflows/action-test-macos.yml/badge.svg)](https://github.com/GuillaumeFalourd/stk-cli-action-poc/actions/workflows/action-test-macos.yml) [![Action test Windows](https://github.com/GuillaumeFalourd/stk-cli-action-poc/actions/workflows/action-test-windows.yml/badge.svg)](https://github.com/GuillaumeFalourd/stk-cli-action-poc/actions/workflows/action-test-windows.yml)

GitHub action to install StackSpot CLI :octocat:

## 📚 Usage

_**Note**: This action is supported on all runners operating systems (`ubuntu`, `macos`, `windows`)_

```yaml
    steps:
      - uses: GuillaumeFalourd/stk-cli-action-poc@main

      - run: stk login --client-id=$CLIENT_ID --client-key=$CLIENT_KEY --realm=$REALM 
        env:
          CLIENT_ID: ${{ secrets.CLIENT_ID}}
          CLIENT_KEY: ${{ secrets.CLIENT_KEY}}
          REALM: ${{ secrets.REALM}}

      - run: stk --version
```
