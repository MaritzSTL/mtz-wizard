[![Build Status](https://img.shields.io/travis/MaritzSTL/mtz-wizard/master.svg?style=flat-square)](https://travis-ci.org/MaritzSTL/mtz-wizard)
[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg?style=flat-square)](https://www.webcomponents.org/element/MaritzSTL/mtz-wizard)

# \<mtz-wizard\>
Generates a wizard flow from steps provided. Allows for validation across all steps.

<!--
```
<custom-element-demo>
  <template>
    <link rel="import" href="../iron-form/iron-form.html">
    <link rel="import" href="mtz-wizard.html">
    <link rel="import" href="mtz-wizard-step.html">
    <link rel="import" href="mtz-wizard-stepper.html">

    <next-code-block></next-code-block>
  </template>
</custom-element-demo>
```
-->
```html
<mtz-wizard-stepper steps="[[steps]]" selected="{{selected}}"></mtz-wizard-stepper>
<mtz-wizard>
  <mtz-wizard-step name="step-1" label="Select campaign settings">
    Step 1 - Prebuilt step
  </mtz-wizard-step>
  <div wizard-step name="step-2" label="Create ad" invalid>
    Step 2 - Generic div using attribute w/ invalid styling applied
  </div>
  <mtz-wizard-step name="step-3" label="Preview ad" optional>
    <iron-form wizard-form>
      <form>
        <label>
          Age:
          <input required type="number" name="age" />
        </label>
      </form>
    </iron-form>
  </mtz-wizard-step>
</mtz-wizard>
```

## Install the Polymer-CLI

First, make sure you have the [Polymer CLI](https://www.npmjs.com/package/polymer-cli) installed. Then run `polymer install --variants` to install all dependencies for both 1.x and 2.x (mainline)

## Viewing Your Element

```
$ polymer serve
```

## Running Tests

```
$ polymer test
```

Your application is already set up to be tested via [web-component-tester](https://github.com/Polymer/web-component-tester). Run `polymer test` to run your application's test suite locally.
