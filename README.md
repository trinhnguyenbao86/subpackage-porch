This is a simple example of subpackage validation in Porch. 

We structure the package into 2 levels:
**1. At parent level**
  - _parent-parameters.yaml_ file contains the parameters that will be then passed to _subpackage-parameters.yaml_ file
  - _fn-pass-parameters.yaml_ file specify the Kpt function (written in Starlark) that is used to pass parameters in _parent-parameters.yaml_ file to _subpackage-parameters.yaml_ file

**2. At subpackage level**
  - _subpackage-parameters.yaml_ file receives parameters from _parent-parameters.yaml_ file
  - Then, _config_map.yaml_ file is generated (via invoking _fn-config.yaml_ function) based on the updated _subpackage-parameters.yaml_ file
