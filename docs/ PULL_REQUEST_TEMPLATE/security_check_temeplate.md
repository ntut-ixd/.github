## Security checklist (only for leader check)

- [ ] No backdoor risk
  - Check for unknown network request urls, and script/shell files with unclear purposes,
  - The backend service cannot expose leaked data interfaces for various reasons (even for testing purposes)
- [ ] No network communication protocol risk
  - Check whether to introduce unsafe network calls such as http/ws
- [ ] No import potentially risk 3rd library
  - Check whether 3rd dependent library is import
  - Don't use an unknown third-party library
  - Check the 3rd library sources are fetched from normal sources, such as npm, gomodule, maven, cocoapod, Do not use unknown sources
  - Check github Dependabot alerts, Whether to add new issues
- [ ] Private data not exposed
  - Check whether there are exclusive ApiKey, privatekey and other private information uploaded to git
  - Check if the packaged keystore has been uploaded to git
