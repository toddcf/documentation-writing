# 1: Form Loads

## Pages

*All pages containing forms.*

## Analytics

- All Form Load & Event analytics from [Forms](../forms.md).
- Plus:
  - events:
    - 'form-load'

## Application Implementation

If a page contains a form, it can load in two ways:

1. The form loads automatically when the page loads.
2. The form is revealed by the user's interaction with the page.

In either case, set the data layer as follows:

- All Form Load implementation from [Forms](../forms.md).
- Plus:
  - digitalData:
    - form:
      - status: 'load'

Then, *if the form was loaded separately from the page load*, dispatch event **'global-form-event'**.