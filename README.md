# ansible-molecule-action

GitHub Action to run Molecule

## Usage

```yaml
name: Run Ansible Molecule

on:
  push:
  pull_request:
    branches:
      - master

jobs:
  build:
    runs-on: ubuntu-latest

    steps:
      - name: Checkout
        uses: actions/checkout@v2

      - name: Run Ansible Molecule
        uses: hspaans/ansible-molecule-action@v0.1.0
```
