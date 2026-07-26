# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: cbp-editor\testing.spec.ts >> creating basic cbp
- Location: tests\cbp-editor\testing.spec.ts:4:5

# Error details

```
TimeoutError: locator.click: Timeout 30000ms exceeded.
Call log:
  - waiting for getByRole('button', { name: 'Basic' })

```

# Page snapshot

```yaml
- generic [ref=e1]:
  - generic:
    - generic:
      - generic:
        - navigation [ref=e2]:
          - generic [ref=e3]:
            - button [ref=e6] [cursor=pointer]
            - list [ref=e8]:
              - listitem [ref=e9]:
                - list [ref=e11]:
                  - button [ref=e13] [cursor=pointer]:
                    - img [ref=e14]
                  - listitem [ref=e18]:
                    - button [ref=e19] [cursor=pointer]:
                      - img [ref=e20]
        - generic:
          - generic:
            - generic:
              - generic:
                - generic [ref=e27]:
                  - generic [ref=e28]:
                    - generic [ref=e30]:
                      - button " Action " [ref=e31] [cursor=pointer]:
                        - generic [ref=e32]: 
                        - generic [ref=e33]: Action
                        - generic [ref=e34]: 
                      - text:     
                    - img [ref=e37]
                  - generic [ref=e43]:
                    - button [ref=e44] [cursor=pointer]:
                      - img [ref=e46]
                    - button [ref=e50] [cursor=pointer]:
                      - img [ref=e52]
                    - button [ref=e56] [cursor=pointer]:
                      - img [ref=e58]
                    - button [ref=e62] [cursor=pointer]:
                      - img [ref=e64]
                    - button [ref=e69] [cursor=pointer]:
                      - img [ref=e71]
                    - button [ref=e77] [cursor=pointer]:
                      - img [ref=e79]
                    - button [ref=e85] [cursor=pointer]:
                      - img [ref=e88]
                    - button [ref=e93] [cursor=pointer]:
                      - img [ref=e95]
                  - generic [ref=e101]:
                    - button "Preview" [ref=e102] [cursor=pointer]:
                      - generic [ref=e103]: 
                      - generic [ref=e104]: Preview
                    - button "Save CBP" [ref=e105] [cursor=pointer]:
                      - generic [ref=e106]: 
                      - generic [ref=e107]: Save CBP
                - generic [ref=e109]:
                  - text:                                                                 
                  - generic [ref=e111]:
                    - generic [ref=e113]:
                      - list [ref=e116]:
                        - listitem [ref=e117]:
                          - generic [ref=e118] [cursor=pointer]: Index
                        - listitem [ref=e119]:
                          - generic [ref=e120] [cursor=pointer]: Control
                        - listitem [ref=e121]:
                          - generic [ref=e123] [cursor=pointer]: Reference
                      - generic [ref=e124]:
                        - generic [ref=e125]: PAGE
                        - generic [ref=e126] [cursor=pointer]:
                          - img [ref=e127]
                          - generic [ref=e130]: Cover Page
                        - generic [ref=e131]: SECTIONS
                        - list [ref=e136]:
                          - listitem [ref=e137]:
                            - generic [ref=e139] [cursor=pointer]: "1.0"
                    - text:                                                               
                  - generic [ref=e147] [cursor=pointer]:
                    - generic [ref=e148]:
                      - img [ref=e149]:
                        - img [ref=e150]
                      - generic [ref=e154]: "1.0"
                    - generic [ref=e157]:
                      - textbox "Section HEADER" [active] [ref=e158]
                      - generic [ref=e160]: 
                  - generic [ref=e166]:
                    - generic [ref=e167]:
                      - img [ref=e169]
                      - generic [ref=e172]: Property Section
                    - generic [ref=e175]:
                      - generic [ref=e176]:
                        - generic [ref=e177]: Type
                        - generic [ref=e178]:
                          - generic:
                            - generic:
                              - generic: Section
                              - generic:
                                - img
                      - generic [ref=e179]:
                        - generic [ref=e180]: Number
                        - paragraph [ref=e181]: "1.0"
                      - generic [ref=e183]:
                        - text: UniqueID
                        - textbox [disabled] [ref=e184]: "1"
                      - generic [ref=e186] [cursor=pointer]:
                        - checkbox "Numbered Sequence" [checked] [ref=e187]
                        - generic [ref=e188]: Numbered Sequence
                      - generic [ref=e190] [cursor=pointer]:
                        - checkbox "Acknowledgement Required" [ref=e191]
                        - generic [ref=e192]: Acknowledgement Required
                      - generic [ref=e194]:
                        - generic [ref=e195]:
                          - generic [ref=e196]: Usage
                          - generic [ref=e199] [cursor=pointer]:
                            - generic [ref=e200]: Continuous
                            - img [ref=e202]
                        - generic [ref=e204]:
                          - generic [ref=e205]: Dependency
                          - generic [ref=e208] [cursor=pointer]:
                            - generic [ref=e209]: Default
                            - img [ref=e211]
                      - generic [ref=e213]:
                        - button "Applicability Rules" [ref=e215] [cursor=pointer]
                        - button "Role/Qualification" [ref=e217] [cursor=pointer]
```

# Test source

```ts
  1  | import { test } from '@playwright/test';
  2  | import { HomePage } from '../../src/pages/HomePage';
  3  | 
  4  | test('creating basic cbp', async ({ page }) =>{
  5  |   const homePage = new HomePage(page);
  6  |   
  7  |   // Navigate to homepage and open CBP Editor module
  8  |   await homePage.openCBPEditor();
  9  | await page.getByRole('textbox', { name: 'Section HEADER' }).click();
> 10 | await page.getByRole('button', { name: 'Basic' }).click();
     |                                                   ^ TimeoutError: locator.click: Timeout 30000ms exceeded.
  11 | //await page.locator('a').filter({ hasText: 'Control' }).first()
  12 | 
  13 | });
```