# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: cbp-editor\basic.cbpeditor.spec.ts >> creating basic cbp
- Location: tests\cbp-editor\basic.cbpeditor.spec.ts:4:5

# Error details

```
TimeoutError: locator.click: Timeout 30000ms exceeded.
Call log:
  - waiting for locator('button.dropbtn > app-action-icon.stickyNote > svg')

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
                      - text:   
                    - img [ref=e37]
                  - generic [ref=e45]:
                    - generic [ref=e46]:
                      - generic [ref=e47]:
                        - button "img" [ref=e48] [cursor=pointer]:
                          - img "img" [ref=e49]
                        - text:         
                      - button [ref=e51] [cursor=pointer]:
                        - img [ref=e53]
                      - generic [ref=e56]:
                        - button "img" [ref=e57] [cursor=pointer]:
                          - img "img" [ref=e58]
                        - text:       
                    - button [ref=e60] [cursor=pointer]:
                      - img [ref=e63]
                    - button [ref=e68] [cursor=pointer]:
                      - img [ref=e70]
                  - generic [ref=e76]:
                    - button "Preview" [ref=e77] [cursor=pointer]:
                      - generic [ref=e78]: 
                      - generic [ref=e79]: Preview
                    - button "Save CBP" [ref=e80] [cursor=pointer]:
                      - generic [ref=e81]: 
                      - generic [ref=e82]: Save CBP
                - generic [ref=e84]:
                  - text:                                                                 
                  - generic [ref=e86]:
                    - generic [ref=e88]:
                      - list [ref=e91]:
                        - listitem [ref=e92]:
                          - generic [ref=e93] [cursor=pointer]: Index
                        - listitem [ref=e94]:
                          - generic [ref=e95] [cursor=pointer]: Control
                        - listitem [ref=e96]:
                          - generic [ref=e98] [cursor=pointer]: Reference
                      - generic [ref=e100]:
                        - generic [ref=e101]:
                          - heading "Basic" [level=5] [ref=e103]:
                            - button "Basic" [ref=e104] [cursor=pointer]
                          - generic [ref=e106]:
                            - generic: Section
                            - generic: Sub Section
                            - generic:
                              - generic: 
                              - text: Action Step
                            - generic:
                              - generic: 
                              - text: Signature Step
                            - generic:
                              - generic: 
                              - text: Information Step
                            - generic:
                              - generic: 
                              - text: Delay Step
                            - generic:
                              - generic: 
                              - text: Timed Step
                            - generic:
                              - generic: 
                              - text: Repeat Step
                            - generic:
                              - generic: 
                              - text: Hold Step
                            - generic:
                              - generic: 
                              - text: Dual Step
                            - generic:
                              - generic: 
                              - text: Procedure Snippet
                            - generic:
                              - generic:
                                - img
                              - text: Warning
                              - generic:
                                - generic: 
                            - generic:
                              - generic:
                                - img
                              - text: Caution
                              - generic:
                                - generic: 
                            - generic:
                              - generic:
                                - img
                              - text: Note
                              - generic:
                                - generic: 
                            - generic:
                              - generic:
                                - img
                              - text: Alara
                              - generic:
                                - generic: 
                            - generic [ref=e107]:
                              - generic [ref=e108]: 
                              - text: Label
                              - generic [ref=e110]: 
                            - generic [ref=e111]:
                              - generic [ref=e112]: 
                              - text: Paragraph
                              - generic [ref=e114]: 
                            - generic:
                              - generic: 
                              - text: Formula
                              - generic:
                                - generic: 
                        - heading "Data Entry" [level=5] [ref=e117]:
                          - button "Data Entry" [ref=e118] [cursor=pointer]
                        - heading "Reference/Link" [level=5] [ref=e121]:
                          - button "Reference/Link" [ref=e122] [cursor=pointer]
                        - heading "Verification" [level=5] [ref=e125]:
                          - button "Verification" [ref=e126] [cursor=pointer]
                    - text:                                            
                  - generic [ref=e130]:
                    - generic [ref=e134] [cursor=pointer]:
                      - generic [ref=e135]:
                        - img [ref=e136]:
                          - img [ref=e137]
                        - generic [ref=e141]: "1.0"
                      - generic [ref=e142]:
                        - textbox "Section HEADER" [ref=e145]
                        - table [ref=e154]:
                          - rowgroup [ref=e155]:
                            - row "Column1 Column2 Column3 Column4" [ref=e156]:
                              - columnheader "Column1" [ref=e157]:
                                - generic [ref=e158]: Column1
                              - columnheader "Column2" [ref=e160]:
                                - generic [ref=e161]: Column2
                              - columnheader "Column3" [ref=e163]:
                                - generic [ref=e164]: Column3
                              - columnheader "Column4" [ref=e166]:
                                - generic [ref=e167]: Column4
                          - rowgroup [ref=e168]:
                            - row [ref=e169]:
                              - cell [ref=e170]
                              - cell [ref=e172]
                              - cell [ref=e174]
                              - cell [ref=e176]
                            - row [ref=e178]:
                              - cell [ref=e179]
                              - cell [ref=e181]
                              - cell [ref=e183]
                              - cell [ref=e185]
                            - row [ref=e187]:
                              - cell [ref=e188]
                              - cell [ref=e190]
                              - cell [ref=e192]
                              - cell [ref=e194]
                            - row [ref=e196]:
                              - cell [ref=e197]
                              - cell [ref=e199]
                              - cell [ref=e201]
                              - cell [ref=e203]
                            - row [ref=e205]:
                              - cell [ref=e206]
                              - cell [ref=e208]
                              - cell [ref=e210]
                              - cell [ref=e212]
                    - generic [ref=e217] [cursor=pointer]:
                      - generic [ref=e218]:
                        - img [ref=e219]:
                          - img [ref=e220]
                        - generic [ref=e224]: "2.0"
                      - textbox "Section HEADER" [ref=e228]
                    - generic [ref=e230]:
                      - generic [ref=e234] [cursor=pointer]:
                        - generic [ref=e235]:
                          - img [ref=e236]:
                            - img [ref=e237]
                          - generic [ref=e242]: "2.1"
                        - textbox "Sub Section HEADER" [ref=e246]
                      - generic [ref=e252] [cursor=pointer]:
                        - generic [ref=e253]:
                          - generic [ref=e254]: 
                          - generic [ref=e257]: 2.1.1
                        - generic [ref=e258]:
                          - textbox "Action Step HEADER" [ref=e261]
                          - table [ref=e273]:
                            - rowgroup [ref=e274]:
                              - row "Column1 Column2 Column3 Column4" [ref=e275]:
                                - columnheader "Column1" [ref=e276]:
                                  - generic [ref=e277]: Column1
                                - columnheader "Column2" [ref=e278]:
                                  - generic [ref=e279]: Column2
                                - columnheader "Column3" [ref=e280]:
                                  - generic [ref=e281]: Column3
                                - columnheader "Column4" [ref=e282]:
                                  - generic [ref=e283]: Column4
                            - rowgroup [ref=e284]:
                              - row [ref=e285]:
                                - cell [ref=e286]
                                - cell [ref=e288]
                                - cell [ref=e290]
                                - cell [ref=e292]
                              - row [ref=e294]:
                                - cell [ref=e295]
                                - cell [ref=e297]
                                - cell [ref=e299]
                                - cell [ref=e301]
                  - generic [ref=e308]:
                    - generic [ref=e309]:
                      - img [ref=e311]
                      - generic [ref=e314]: Property Table
                    - generic [ref=e317]:
                      - generic [ref=e318]:
                        - generic [ref=e319]: Data Type
                        - textbox [ref=e320]: Table
                      - generic [ref=e321]:
                        - generic [ref=e322]: Table Name
                        - textbox "Table Name" [ref=e323]: Table22
                      - generic [ref=e325]:
                        - text: UniqueID
                        - textbox [disabled] [ref=e326]: "21"
                      - generic [ref=e328]:
                        - button "Table Rule" [ref=e330] [cursor=pointer]
                        - generic [ref=e333]:
                          - generic [ref=e334] [cursor=pointer]: Exclude Rows
                          - spinbutton [ref=e335]: "0"
```

# Test source

```ts
  1   | import { test } from '@playwright/test';
  2   | import { HomePage } from '../../src/pages/HomePage';
  3   | 
  4   | test('creating basic cbp', async ({ page }) =>{
  5   |   const homePage = new HomePage(page);
  6   |   
  7   |   // Navigate to homepage and open CBP Editor module
  8   |   await homePage.openCBPEditor();
  9   |  
  10  |   await page.getByRole('textbox', { name: 'Section HEADER' }).click();
  11  |   await page.getByText('Control', { exact: true }).nth(4).click();
  12  |   await page.getByText('Section', { exact: true }).nth(3).click();
  13  |   await page.locator('#step1').click();
  14  |   await page.locator('#step2').click();
  15  |   await page.getByText('Sub Section').nth(2).click();
  16  |   await page.getByRole('textbox', { name: 'Sub Section HEADER' }).click();
  17  |   await page.getByText('Action Step').nth(1).click();
  18  |   await page.locator('#step1').click();
  19  |   await page.getByRole('button', { name: ' Action ' }).click();
  20  |   await page.locator('a').filter({ hasText: 'Add' }).click();
  21  |   await page.getByRole('button', { name: ' Action ' }).click();
  22  |   await page.locator('a').filter({ hasText: 'Add' }).click();
  23  |   await page.locator('a').filter({ hasText: 'Data Entry' }).click();
  24  |   await page.getByText('Table').click();
  25  |   await page.getByRole('spinbutton').first().click();
  26  |   await page.getByRole('spinbutton').first().fill('4');
  27  |   await page.getByRole('spinbutton').first().click();
  28  |   await page.getByRole('spinbutton').first().fill('4');
  29  |   await page.getByRole('button', { name: 'Ok', exact: true }).click();
  30  |   
  31  |   // Click OK button in the table properties dialog to close it
  32  |   await page.locator('#tablePropertie').getByRole('button', { name: 'Ok', exact: true }).click();
  33  |   
  34  |   await page.locator('#step1').click();
  35  |   await page.getByRole('button', { name: ' Action ' }).click();
  36  |   await page.locator('a').filter({ hasText: 'Add' }).click();
  37  |   await page.locator('a').filter({ hasText: 'Data Entry' }).click();
  38  |   await page.locator('a').filter({ hasText: 'Data Entry' }).click();
  39  |   await page.getByText('Table').click();
  40  |   await page.getByRole('spinbutton').first().click();
  41  |   await page.getByRole('spinbutton').nth(1).click();
  42  |   await page.getByRole('spinbutton').nth(1).click();
  43  |   await page.getByRole('spinbutton').nth(1).click();
  44  |   await page.getByRole('spinbutton').first().click();
  45  |   await page.getByRole('spinbutton').first().click();
  46  |   await page.getByRole('spinbutton').first().fill('4');
  47  |   await page.getByRole('spinbutton').nth(1).click();
  48  |   await page.getByRole('spinbutton').nth(1).fill('5');
  49  |   await page.getByRole('button', { name: 'Ok' }).click();
  50  |   
  51  |   // Wait for and close the table properties dialog
  52  |   await page.locator('#tablePropertie').getByRole('button', { name: 'Ok', exact: true }).click();
  53  |   await page.waitForTimeout(1000); // Wait for dialog to close
  54  |   
  55  |   // Skip column configuration - table structure may vary
  56  |   // await page.getByText('Column', { exact: true }).click();
  57  |   // ... column configuration steps ...
  58  |   
> 59  |   await page.locator(`button.dropbtn > app-action-icon.stickyNote > svg`).click();
      |                                                                           ^ TimeoutError: locator.click: Timeout 30000ms exceeded.
  60  |   //await page.getByRole('button', { description: 'Sticky Note', exact: true }).click();
  61  |   await page.getByRole('textbox', { name: 'Enter your comments here' }).click();
  62  |   await page.getByRole('textbox', { name: 'Enter your comments here' }).fill('to proceed check the warnings');
  63  |   await page.getByRole('button', { name: 'submit' }).click();
  64  |   await page.locator('.fa.fa-times').first().click();
  65  |   await page.locator('#step2').click();
  66  |   await page.getByRole('button', { description: 'Alert', exact: true }).click();
  67  |   await page.getByRole('button', { description: 'Warning', exact: true }).click();
  68  |   await page.getByRole('button', { description: 'Alert', exact: true }).click();
  69  |   await page.getByRole('button', { description: 'Caution', exact: true }).click();
  70  |   await page.getByRole('button', { description: 'Alert', exact: true }).click();
  71  |   await page.getByRole('button', { description: 'Alert', exact: true }).click();
  72  |   await page.getByRole('button', { description: 'Note', exact: true }).click();
  73  |   await page.locator('#step2').click();
  74  |   await page.getByRole('button', { name: ' Action ' }).click();
  75  |   await page.locator('a').filter({ hasText: 'Add' }).click();
  76  |   await page.locator('a').filter({ hasText: 'Signature Step' }).click();
  77  |   await page.locator('#step2').click();
  78  |   await page.getByRole('button', { name: ' Action ' }).click();
  79  |   await page.locator('a').filter({ hasText: 'Note' }).click();
  80  |   await page.locator('#note-17847913103150').click();
  81  |   await page.locator('#note-17847913103150').fill('');
  82  |   await page.locator('#note-17847913103150').click();
  83  |   await page.locator('#note-17847913103150').fill('cbp editor');
  84  |   await page.locator('#step1').click();
  85  |   await page.locator('div:nth-child(12) > button').click();
  86  |   await page.locator('.buttns.w-auto').first().click();
  87  |   await page.getByRole('button', { name: 'Choose File' }).setInputFiles(['1.jpg', '2025-03-18_092834.png', 'DAy.jpg', 'DG.png.png', 'girl-with-red-hat-BBZDOHhYU2s-unsplash.jpg', 'Greenary.jpg', 'Header Logo7257437.png', '-icon-logo.png', 'Image.jpg', 'istockphoto-1152614033-612x612.jpg', 'jpeg.jfif', 'jpeg1.jfif', 'jpeg2.jfif', 'jpeg3.jfif', 'jpeg4.jpg', 'jpeg5.jpg', 'jpeg6.jfif', 'jpeg7.jpg', 'jpeg8.jpg', 'jpeg9.jpeg', 'JPG.jpg', 'Keep Going.jpg', 'Motivational-quotes-image-for-work-768x432.jpg.jpg', 'PNG.png', 'PNG2.jfif', 'River.jpg', 'Robot.jpg', 'Soft.jpg', 'software.jpg', 'Success.jpg', 'Sunrise.jpg', 'Tata.jpg', 'Test.jpeg', 'tiger jpeg.jfif', 'Tree.jpg', 'Water.jpg', 'you did it!.jpg']);
  88  |   await page.locator('#step1').click();
  89  |   await page.locator('div:nth-child(12) > button').click();
  90  |   await page.locator('.d-flex > button:nth-child(3)').click();
  91  |   await page.locator('#fileUploadMedia').setInputFiles('DG.png.png');
  92  |   await page.getByRole('combobox').selectOption('center');
  93  |   await page.locator('.btn-trans.btn.btn-icon.ng-star-inserted').click();
  94  |   await page.getByRole('textbox').nth(1).fill('dataglance');
  95  |   await page.locator('.ng-resizable-handle').click();
  96  |   await page.locator('#scrollSection3 #stop_draging_id').click();
  97  |   await page.locator('.fa.fa-edit').click();
  98  |   await page.locator('#cbp-editor').click();
  99  |   await page.locator('#cbp-editor').fill('Enter text properly');
  100 |   await page.getByRole('textbox', { name: 'Action Step HEADER' }).click();
  101 |   await page.getByRole('button', { name: 'Basic' }).click();
  102 |   await page.getByRole('button', { name: 'Basic' }).click();
  103 |   await page.getByText('Signature Step').nth(2).click();
  104 | });
  105 | 
```