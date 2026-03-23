# Example Wombat Action

This is an example action to demonstrate the structure of actions within the `wombat-actions` repository.

## Inputs

| Name            | Description  | Required | Default |
| --------------- | ------------ | -------- | ------- |
| `greeting_name` | Who to greet | `true`   | `World` |

## Outputs

| Name            | Description                          |
| --------------- | ------------------------------------ |
| `greeting_time` | The time the greeting was generated. |

## Usage

```yaml
jobs:
  example_job:
    runs-on: ubuntu-latest
    name: A job to say hello
    steps:
      - uses: actions/checkout@v4
      - name: Example Action Step
        uses: ./example-action
        with:
          greeting_name: "Wombat Fan"
```
