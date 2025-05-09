# Starlark KPT Function Test

## How to Run

1. Make sure you have kpt installed.
2. cd into this folder.
3. Run the command:

   kpt fn eval . --image gcr.io/kpt-fn/starlark:v0.5.0 --fn-config fn-config.yaml

4. Then check the file `configmap.yaml` to see if `new-key: new-value` was added.
