# Forms

## Pages

*Any page on the site that contains a form.*

## Analytics

### Form Loads & Events

- All *Event* analytics from [Global](../global.md).
- Plus:
  - eVar13 (Form Type): digitalData.form.type
  - eVar14 (Form Name): digitalData.form.name
  - eVar15 (Form Code): digitalData.form.id

## Application Implementation

### Form Loads

Populate the data layer according to the documentation for that page's form:

- digitalData:
  - form:
    - id: (string: form code)
    - name: (string)
    - type: (string: 'lead-gen', 'account', etc.)