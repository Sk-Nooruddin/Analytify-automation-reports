# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: cbp-editor\flow.cbpedito.spec.ts >> creating basic cbp
- Location: tests\cbp-editor\flow.cbpedito.spec.ts:5:5

# Error details

```
TimeoutError: locator.click: Timeout 30000ms exceeded.
Call log:
  - waiting for getByRole('button', { name: 'Add' })

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
                            - generic [ref=e139] [cursor=pointer]: 1.0 Section
                    - text:                                                               
                  - generic [ref=e147] [cursor=pointer]:
                    - generic [ref=e148]:
                      - img [ref=e149]:
                        - img [ref=e150]
                      - generic [ref=e154]: "1.0"
                    - generic [ref=e157]:
                      - textbox "Section HEADER" [active] [ref=e158]: Section
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
  1   | import { test, expect } from '@playwright/test';
  2   | import { CommonPage } from '../../src/pages/CommonPage';
  3   | import { HomePage } from '../../src/pages/HomePage';
  4   | 
  5   | test('creating basic cbp', async ({ page }) =>{
  6   |   const homePage = new HomePage(page);
  7   |   
  8   |   // Navigate to homepage and open CBP Editor module
  9   |   await homePage.openCBPEditor();
  10  |  
  11  |   
  12  | //await page.getByPlaceholder("Section HEADER").click();  
  13  | //await page.locator('css=[#id="step1"]').click();  
  14  | //await page.getByRole('textbox', { name: 'Section header' }).fill('section header');
  15  | //await page.getAttribute('class=pointer fontSize-Index responsiveFont checkactive', 'aria-disabled');
  16  | //await page.locator('text=CBP Editor').click();
  17  | //await page.getByRole('textbox')
  18  |   await page.getByRole('textbox', { name: 'Section HEADER' }).fill('Section');
  19  |  // await page.locator('a').filter({ hasText: 'Sub Section' }).click();
  20  | const addButton = page.getByRole('button', { name: 'Add' });
> 21  | await addButton.click();
      |                 ^ TimeoutError: locator.click: Timeout 30000ms exceeded.
  22  | 
  23  | 
  24  | const subSection = page.locator('a:has-text("Sub Section")');
  25  | await expect(subSection).toBeVisible();
  26  | await subSection.click();
  27  | await page.waitForTimeout(2000);
  28  | 
  29  |   //await page.getByRole('textbox', { name: 'Sub Section' }).click();
  30  |   await page.getByRole('textbox', { name: 'Sub Section HEADER' }).fill('Sub section');
  31  |   
  32  |   await page.getByRole('textbox', { name: 'Section HEADER', exact: true }).click();
  33  |   await addButton.click();
  34  |   await page.waitForTimeout(2000);
  35  |   await page.locator('a').filter({ hasText: 'Step Action' }).click();
  36  |   await page.getByRole('textbox', { name: 'StepAction HEADER' }).click();
  37  |   await page.getByRole('textbox', { name: 'StepAction HEADER' }).fill('Step action');
  38  |   await page.getByRole('textbox', { name: 'Section HEADER', exact: true }).click();
  39  |   await addButton.click();
  40  |   await page.waitForTimeout(2000);
  41  |   await page.locator('a').filter({ hasText: 'Signature Step' }).click();
  42  |   await page.getByRole('textbox', { name: 'SignatureStep HEADER' }).click();
  43  |   await page.getByRole('textbox', { name: 'SignatureStep HEADER' }).fill('ignature step');
  44  |   await page.getByRole('textbox', { name: 'SignatureStep HEADER' }).click();
  45  |   await page.getByRole('textbox', { name: 'SignatureStep HEADER' }).fill('ignature step');
  46  |   await page.getByRole('textbox', { name: 'SignatureStep HEADER' }).press('ArrowLeft');
  47  |   await page.getByRole('textbox', { name: 'SignatureStep HEADER' }).press('ArrowLeft');
  48  |   await page.getByRole('textbox', { name: 'SignatureStep HEADER' }).press('ArrowLeft');
  49  |   await page.getByRole('textbox', { name: 'SignatureStep HEADER' }).press('ArrowLeft');
  50  |   await page.getByRole('textbox', { name: 'SignatureStep HEADER' }).press('ArrowLeft');
  51  |   await page.getByRole('textbox', { name: 'SignatureStep HEADER' }).press('ArrowLeft');
  52  |   await page.getByRole('textbox', { name: 'SignatureStep HEADER' }).fill('Signature step');
  53  |   await page.getByRole('textbox', { name: 'Section HEADER', exact: true }).click();
  54  |   await addButton.click();
  55  |   await page.waitForTimeout(2000);
  56  |   await page.locator('a').filter({ hasText: 'StepInfo' }).click();
  57  |   await page.getByRole('textbox', { name: 'StepInfo HEADER' }).click();
  58  |   await page.getByRole('textbox', { name: 'StepInfo HEADER' }).fill('Step info');
  59  |   await page.getByRole('textbox', { name: 'Section HEADER', exact: true }).click();
  60  |   await addButton.click();
  61  |   await page.waitForTimeout(2000);
  62  |   await page.locator('a').filter({ hasText: 'Delay Step' }).click();
  63  |   await page.getByRole('textbox', { name: 'DelayStep HEADER' }).click();
  64  |   await page.getByRole('textbox', { name: 'DelayStep HEADER' }).fill('Delay step');
  65  |   await page.getByRole('textbox', { name: 'Section HEADER', exact: true }).click();
  66  |   await addButton.click();
  67  |   await page.waitForTimeout(2000);
  68  |   await page.locator('a').filter({ hasText: 'Timed Step' }).click();
  69  |   await page.getByRole('textbox', { name: 'Timed HEADER' }).click();
  70  |   await page.getByRole('textbox', { name: 'Timed HEADER' }).fill('Timed step');
  71  |   await page.getByRole('textbox', { name: 'Section HEADER', exact: true }).click();
  72  |   await addButton.click();
  73  |   await page.waitForTimeout(2000);
  74  |   await page.locator('a').filter({ hasText: 'Repeat Step' }).click();
  75  |   await page.getByRole('textbox', { name: 'Repeat HEADER' }).click();
  76  |   await page.getByRole('textbox', { name: 'Repeat HEADER' }).fill('Repeat step');
  77  |   await page.getByRole('textbox', { name: 'Section HEADER', exact: true }).click();
  78  |   await addButton.click();
  79  |   await page.waitForTimeout(2000);
  80  |   await page.locator('a').filter({ hasText: 'Hold Step' }).click();
  81  |   await page.getByRole('textbox', { name: 'HoldStep HEADER' }).click();await addButton.click();
  82  |   await page.getByRole('textbox', { name: 'HoldStep HEADER' }).fill('Hold step');
  83  |   await page.getByRole('textbox', { name: 'Section HEADER', exact: true }).click();
  84  |   await addButton.click();
  85  |   await page.waitForTimeout(2000);
  86  |   await page.locator('a').filter({ hasText: 'Warning' }).click();
  87  |   await page.waitForTimeout(2000);
  88  |   await page.locator('a').filter({ hasText: 'Caution' }).click();
  89  |   await page.waitForTimeout(2000);
  90  |   await page.locator('a').filter({ hasText: 'Note' }).click();
  91  |   await page.waitForTimeout(2000);
  92  |   await page.locator('a').filter({ hasText: 'Alara' }).click();
  93  |   await page.waitForTimeout(2000);
  94  |   await page.locator('a').filter({ hasText: 'Label' }).click();
  95  |   await page.waitForTimeout(2000);
  96  |   await page.locator('a').filter({ hasText: 'Para' }).click();
  97  |   await page.waitForTimeout(2000);
  98  |   await page.locator('a').filter({ hasText: 'Formula' }).click();
  99  |  await page.waitForTimeout(2000);
  100 |    await page.locator('a:has-text("Data Entry")').click();
  101 | 
  102 |   await page.waitForTimeout(2000);
  103 |   await page.locator('a:has-text("Table")').click();
  104 |     await page.waitForTimeout(2000);
  105 | const columnInput = page.locator('div.row:has-text("Number of Columns")').locator('input[type="number"]');
  106 | await columnInput.fill('5');
  107 | const rowInput = page.locator('div.row:has-text("Number of Rows") input[type="number"]');
  108 | await rowInput.fill('5');
  109 | //await page.getByRole('link', { name: 'Table' }).click();
  110 | 
  111 | });
```