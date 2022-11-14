# stk-cli-action-poc

[![Action test Ubuntu](https://github.com/GuillaumeFalourd/stk-cli-action-poc/actions/workflows/action-test-ubuntu.yml/badge.svg)](https://github.com/GuillaumeFalourd/stk-cli-action-poc/actions/workflows/action-test-ubuntu.yml) [![Action test MacOS](https://github.com/GuillaumeFalourd/stk-cli-action-poc/actions/workflows/action-test-macos.yml/badge.svg)](https://github.com/GuillaumeFalourd/stk-cli-action-poc/actions/workflows/action-test-macos.yml) [![Action test Windows](https://github.com/GuillaumeFalourd/stk-cli-action-poc/actions/workflows/action-test-windows.yml/badge.svg)](https://github.com/GuillaumeFalourd/stk-cli-action-poc/actions/workflows/action-test-windows.yml)

GitHub action to install StackSpot CLI :octocat:

## 📚 Usage

_**Note**: This action is supported on all runners operating systems (`ubuntu`, `macos`, `windows`)_

```yaml
    steps:
      - uses: GuillaumeFalourd/stk-cli-action-poc@main
        with:
          client_id: ${{ secrets.CLIENT_ID}}
          client_key: ${{ secrets.CLIENT_KEY}}
          realm: ${{ secrets.REALM}}
      - run: stk --version
```
