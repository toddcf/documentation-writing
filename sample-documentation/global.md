# Global

*This sample documentation describes a fictional website for a solar power company.*

## Pages

- / (homepage)
  - /about
  - /account
    - /login
    - /manage
      - /contact-info
      - /preferences
    - /recovery
      - /password
      - /username
    - / registration
  - /cart
    - /summary
    - /payment
    - /confirmation
  - /content
    - /products
      - /batteries
        - /commercial
        - /industrial
        - /residential
      - /solar-panels
        - /commercial
        - /industrial
        - /residential
    - /services
      - /installation
      - /repair
  - /email-list
  - /faq
  - /support

## Analytics

### Page Loads & Events

- eVar1 (Page Level 1): digitalData.page.level1
- eVar2 (Page Level 2): digitalData.page.level2 *(if applicable)*
- eVar3 (Page Level 3): digitalData.page.level3 *(if applicable)*
- eVar4 (Page Level 4): digitalData.page.level4 *(if applicable)*
- eVar5 (Page Level 5): digitalData.page.level5 *(if applicable)*
- eVar6 (Pathname): digitalData.page.pathname
- eVar7 (Country): digitalData.site.country
- eVar8 (Language): digitalData.site.language
- eVar9 (Environment): digitalData.user.auth
- eVar10 (User Auth Status): digitalData.user.auth
- eVar11 (User ID): digitalData.user.id *(if known)*

### Page Loads Only

- All "Page Loads & Events" variables.
- Plus:
  - eVar12 (Page Load Time): digitalData.page.loadTime

## Application Implementation

### Page Loads

Populate the data layer:

- digitalData:
  - page:
    - level1: (string)
    - level2: (string)
    - level3: (string)
    - level4: (string)
    - level5: (string)
    - loadTime: (number: milliseconds)
    - pathname: (string)
  - site:
    - country: (string: 'us', 'gb', 'au', 'nz', 'hk', etc.)
    - env: (string: 'dev', 'stage,' 'prod', etc.)
    - language: (string: 'en', 'es', etc.)
    - region: (string: 'nam', 'uk', 'au', 'intl', etc.)
  - user:
    - auth: (Boolean: **true** if logged in)
    - id: (string: unique identifier) *(if known)*