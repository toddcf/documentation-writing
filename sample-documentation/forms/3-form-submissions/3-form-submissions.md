# 3: Form Submissions

## Pages

*All pages containing forms.*

## Analytics

- All Form Event analytics from [Forms](../forms.md).
- Plus:
  - events:
    - 'form-submit-success' *(if **'global-form-event'** is detected, and if **digitalData.form.status === 'submit-success'**)*

*If form submission fails, it is tracked via [Errors](../../errors/errors).*

## Application Implementation

1. Once the form has been submitted either successfully or unsuccessfully, update the data layer accordingly:
  - digitalData:
    - form:
      - status: 'form-submit-success' vs. 'form-submit-error'
2. Then dispatch **'global-form-event'**.