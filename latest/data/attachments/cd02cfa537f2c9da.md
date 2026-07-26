# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: cbp-editor\testing.spec.ts >> creating basic cbp
- Location: tests\cbp-editor\testing.spec.ts:5:5

# Error details

```
TimeoutError: locator.fill: Timeout 30000ms exceeded.
Call log:
  - waiting for locator('.fb-row').filter({ hasText: 'WARNING' }).getByRole('textbox', { name: 'Enter your cause' })

```

# Page snapshot

```yaml
- generic [active] [ref=e1]:
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
                      - generic [ref=e125]:
                        - generic [ref=e126]:
                          - heading "Basic" [level=5] [ref=e128]:
                            - button "Basic" [ref=e129] [cursor=pointer]
                          - generic [ref=e131]:
                            - generic [ref=e132]: Section
                            - generic [ref=e133]: Sub Section
                            - generic [ref=e134]:
                              - generic [ref=e135]: 
                              - text: Action Step
                            - generic [ref=e136]:
                              - generic [ref=e137]: 
                              - text: Signature Step
                            - generic [ref=e138]:
                              - generic [ref=e139]: 
                              - text: Information Step
                            - generic [ref=e140]:
                              - generic [ref=e141]: 
                              - text: Delay Step
                            - generic [ref=e142]:
                              - generic [ref=e143]: 
                              - text: Timed Step
                            - generic [ref=e144]:
                              - generic [ref=e145]: 
                              - text: Repeat Step
                            - generic [ref=e146]:
                              - generic [ref=e147]: 
                              - text: Hold Step
                            - generic [ref=e148]:
                              - generic [ref=e149]: 
                              - text: Dual Step
                            - generic [ref=e150]:
                              - generic [ref=e151]: 
                              - text: Procedure Snippet
                            - generic [ref=e152]:
                              - img [ref=e154]
                              - text: Warning
                              - generic [ref=e163]: 
                            - generic [ref=e164]:
                              - img [ref=e166]
                              - text: Caution
                              - generic [ref=e170]: 
                            - generic [ref=e171]:
                              - img [ref=e173]
                              - text: Note
                              - generic [ref=e180]: 
                            - generic [ref=e181]:
                              - img [ref=e183]
                              - text: Alara
                              - generic [ref=e201]: 
                            - generic [ref=e202]:
                              - generic [ref=e203]: 
                              - text: Label
                              - generic [ref=e205]: 
                            - generic [ref=e206]:
                              - generic [ref=e207]: 
                              - text: Paragraph
                              - generic [ref=e209]: 
                            - generic [ref=e210]:
                              - generic [ref=e211]: 
                              - text: Formula
                              - generic [ref=e213]: 
                        - heading "Data Entry" [level=5] [ref=e216]:
                          - button "Data Entry" [ref=e217] [cursor=pointer]
                        - heading "Reference/Link" [level=5] [ref=e220]:
                          - button "Reference/Link" [ref=e221] [cursor=pointer]
                        - heading "Verification" [level=5] [ref=e224]:
                          - button "Verification" [ref=e225] [cursor=pointer]
                    - text:                                            
                  - generic [ref=e233] [cursor=pointer]:
                    - generic [ref=e234]:
                      - img [ref=e235]:
                        - img [ref=e236]
                      - generic [ref=e240]: "1.0"
                    - generic [ref=e241]:
                      - generic [ref=e243]:
                        - textbox "Section HEADER" [ref=e244]
                        - generic [ref=e246]: 
                      - generic [ref=e255]:
                        - generic [ref=e256]:
                          - img [ref=e258]
                          - heading "Warning" [level=4] [ref=e266]
                          - img [ref=e268]
                        - generic [ref=e278]:
                          - textbox "Enter your cause" [ref=e281]
                          - textbox "Enter your effect" [ref=e284]
                  - generic [ref=e290]:
                    - generic [ref=e291]:
                      - img [ref=e293]
                      - generic [ref=e296]: Property Section
                    - generic [ref=e299]:
                      - generic [ref=e300]:
                        - generic [ref=e301]: Type
                        - generic [ref=e302]:
                          - generic:
                            - generic:
                              - generic: Section
                              - generic:
                                - img
                      - generic [ref=e303]:
                        - generic [ref=e304]: Number
                        - paragraph [ref=e305]: "1.0"
                      - generic [ref=e307]:
                        - text: UniqueID
                        - textbox [disabled] [ref=e308]: "1"
                      - generic [ref=e310] [cursor=pointer]:
                        - checkbox "Numbered Sequence" [checked] [ref=e311]
                        - generic [ref=e312]: Numbered Sequence
                      - generic [ref=e314] [cursor=pointer]:
                        - checkbox "Acknowledgement Required" [ref=e315]
                        - generic [ref=e316]: Acknowledgement Required
                      - generic [ref=e318]:
                        - generic [ref=e319]:
                          - generic [ref=e320]: Usage
                          - generic [ref=e323] [cursor=pointer]:
                            - generic [ref=e324]: Continuous
                            - img [ref=e326]
                        - generic [ref=e328]:
                          - generic [ref=e329]: Dependency
                          - generic [ref=e332] [cursor=pointer]:
                            - generic [ref=e333]: Default
                            - img [ref=e335]
                      - generic [ref=e337]:
                        - button "Applicability Rules" [ref=e339] [cursor=pointer]
                        - button "Role/Qualification" [ref=e341] [cursor=pointer]
```

# Test source

```ts
  1  | import { test } from '@playwright/test';
  2  | import { HomePage } from '../../src/pages/HomePage';
  3  | import { expect } from '@playwright/test';
  4  | 
  5  | test('creating basic cbp', async ({ page }) =>{
  6  |   const homePage = new HomePage(page);
  7  |   
  8  |   // Navigate to homepage and open CBP Editor module
  9  |   await homePage.openCBPEditor();
  10 | await page.getByRole('textbox', { name: 'Section HEADER' }).click();
  11 | //await page.pause();
  12 | page.getByText('Control', { exact: true }).nth(4).click();
  13 | 
  14 | const source = await page.locator('#cbp_editor_Warning:visible')
  15 | const target = await page.getByRole('textbox', { name: 'Section HEADER' })
  16 | await source.dragTo(target);
  17 | 
  18 | const warning = page.locator('.fb-row').filter({ hasText: 'WARNING' });
  19 | 
  20 | await warning.getByRole('textbox', { name: 'Enter your cause' })
> 21 |   .fill('Warning cause');
     |    ^ TimeoutError: locator.fill: Timeout 30000ms exceeded.
  22 | 
  23 | await warning.getByRole('textbox', { name: 'Enter your effect' })
  24 |   .fill('Warning effect');
  25 | 
  26 | const source1 = await page.locator('#cbp_editor_Caution:visible')
  27 | const target1 = await page.getByRole('textbox', { name: 'Section HEADER' })
  28 | await expect(source1).toBeVisible();
  29 | await source1.scrollIntoViewIfNeeded();
  30 | await source1.dragTo(target1);
  31 | await source1.dragTo(target1);
  32 | 
  33 | const caution = page.locator('.fb-row').filter({ hasText: 'CAUTION' });
  34 | 
  35 | await caution.getByRole('textbox', { name: 'Enter your cause' })
  36 |   .fill('This is a caution cause');
  37 | 
  38 | await caution.getByRole('textbox', { name: 'Enter your effect' })
  39 |   .fill('This is a caution effect');
  40 | 
  41 | const source2 = page.locator('#cbp_editor_Alara:visible')
  42 | const target2 = await page.getByRole('textbox', { name: 'Section HEADER' })
  43 | await expect(source2).toBeVisible();
  44 | await source2.scrollIntoViewIfNeeded();
  45 | await source2.dragTo(target2);
  46 | 
  47 | page.getByRole('textbox', { name: 'Enter your note' }).fill('This is a note message');
  48 | 
  49 | const source3 = page.locator('#cbp_editor_LabelDataEntry:visible')
  50 | const target3 = await page.getByRole('textbox', { name: 'Section HEADER' })
  51 | await expect(source3).toBeVisible();
  52 | await source3.scrollIntoViewIfNeeded();
  53 | await source3.dragTo(target3);
  54 | 
  55 | page.getByRole('textbox', { name: 'Enter your note' }).fill('This is a note message');
  56 | page.locator(".fb-row.stop_draging.ng-star-inserted.section-border").fill('This is a section header message');
  57 | });
```