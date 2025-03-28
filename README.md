# component-random-abstracted
A Pulumi Component Resource (https://www.pulumi.com/docs/iac/concepts/resources/components/) that abstracts the use of the Random provider (https://www.pulumi.com/registry/packages/random/)

It can be used for testing component resources and the "components as components" feature, etc.

# Usage

In the folder of the project code that is using the component, run the following command.
```bash
pulumi package add https://github.com/MitchellGerdisch/component-random-abstracted@v0.1.0
```

# Example Program
The `test-project` folder has an example Pulumi project written in YAML that uses the component.

To use:
* copy the `test-project` to a local folder.
* cd to the test project folder.
* `pulumi package add https://github.com/MitchellGerdisch/component-random-abstracted@v0.1.0`
* `pulumi stack init`
* Modify the code to use one of the allowed sizes (i.e. `small`, `medium`, `large`, `xlarge`) 
* `pulumi up`