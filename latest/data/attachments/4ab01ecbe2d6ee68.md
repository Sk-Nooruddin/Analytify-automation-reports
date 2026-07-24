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
  - waiting for locator('a').filter({ hasText: 'Note' })
    - locator resolved to <a class="cbp-menu-link" _ngcontent-ng-c680531232=""> Note </a>
  - attempting click action
    2 × waiting for element to be visible, enabled and stable
      - element is not visible
    - retrying click action
    - waiting 20ms
    2 × waiting for element to be visible, enabled and stable
      - element is not visible
    - retrying click action
      - waiting 100ms
    58 × waiting for element to be visible, enabled and stable
       - element is not visible
     - retrying click action
       - waiting 500ms

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
                      - button " Action " [active] [ref=e31] [cursor=pointer]:
                        - generic [ref=e32]: 
                        - generic [ref=e33]: Action
                        - generic [ref=e34]: 
                      - text:     
                    - img [ref=e37]
                  - generic [ref=e43]:
                    - button [ref=e44] [cursor=pointer]:
                      - img [ref=e46]
                    - button [ref=e50] [cursor=pointer]:
                      - img [ref=e52]
                    - generic:
                      - button:
                        - generic:
                          - img
                    - button [ref=e56] [cursor=pointer]:
                      - img [ref=e58]
                    - button [ref=e63]:
                      - img [ref=e65]
                    - button [ref=e71] [cursor=pointer]:
                      - img [ref=e73]
                    - button [disabled] [ref=e79]:
                      - img [ref=e82]
                    - button [ref=e87] [cursor=pointer]:
                      - img [ref=e89]
                  - generic [ref=e95]:
                    - button "Preview" [ref=e96] [cursor=pointer]:
                      - generic [ref=e97]: 
                      - generic [ref=e98]: Preview
                    - button "Save CBP" [ref=e99] [cursor=pointer]:
                      - generic [ref=e100]: 
                      - generic [ref=e101]: Save CBP
                - generic [ref=e103]:
                  - text:                                                                 
                  - generic [ref=e105]:
                    - generic [ref=e107]:
                      - list [ref=e110]:
                        - listitem [ref=e111]:
                          - generic [ref=e112] [cursor=pointer]: Index
                        - listitem [ref=e113]:
                          - generic [ref=e114] [cursor=pointer]: Control
                        - listitem [ref=e115]:
                          - generic [ref=e117] [cursor=pointer]: Reference
                      - generic [ref=e119]:
                        - generic [ref=e120]:
                          - heading "Basic" [level=5] [ref=e122]:
                            - button "Basic" [ref=e123] [cursor=pointer]
                          - generic [ref=e125]:
                            - generic [ref=e126]: Section
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
                            - generic [ref=e127]:
                              - generic [ref=e128]: 
                              - text: Label
                              - generic [ref=e130]: 
                            - generic:
                              - generic: 
                              - text: Paragraph
                              - generic:
                                - generic: 
                            - generic:
                              - generic: 
                              - text: Formula
                              - generic:
                                - generic: 
                        - heading "Data Entry" [level=5] [ref=e133]:
                          - button "Data Entry" [ref=e134] [cursor=pointer]
                        - heading "Reference/Link" [level=5] [ref=e137]:
                          - button "Reference/Link" [ref=e138] [cursor=pointer]
                        - heading "Verification" [level=5] [ref=e141]:
                          - button "Verification" [ref=e142] [cursor=pointer]
                    - text:                                            
                  - generic [ref=e146]:
                    - generic [ref=e150] [cursor=pointer]:
                      - generic [ref=e151]:
                        - img [ref=e152]:
                          - img [ref=e153]
                        - generic [ref=e157]: "1.0"
                      - textbox "Section HEADER" [ref=e161]
                    - generic [ref=e173] [cursor=pointer]:
                      - generic [ref=e174]:
                        - img [ref=e175]:
                          - img [ref=e176]
                        - generic [ref=e180]: "2.0"
                      - textbox "Section HEADER" [ref=e184]
                    - generic [ref=e186]:
                      - generic [ref=e190] [cursor=pointer]:
                        - generic [ref=e191]:
                          - img [ref=e192]:
                            - img [ref=e193]
                          - generic [ref=e198]: "2.1"
                        - textbox "Sub Section HEADER" [ref=e202]
                      - generic [ref=e208] [cursor=pointer]:
                        - generic [ref=e209]:
                          - generic [ref=e210]: 
                          - generic [ref=e213]: 2.1.1
                        - generic [ref=e214]:
                          - textbox "Action Step HEADER" [ref=e217]
                          - table [ref=e229]:
                            - rowgroup [ref=e230]:
                              - row "Column1 Column2 Column3 Column4" [ref=e231]:
                                - columnheader "Column1" [ref=e232]:
                                  - generic [ref=e233]: Column1
                                - columnheader "Column2" [ref=e234]:
                                  - generic [ref=e235]: Column2
                                - columnheader "Column3" [ref=e236]:
                                  - generic [ref=e237]: Column3
                                - columnheader "Column4" [ref=e238]:
                                  - generic [ref=e239]: Column4
                            - rowgroup [ref=e240]:
                              - row [ref=e241]:
                                - cell [ref=e242]
                                - cell [ref=e244]
                                - cell [ref=e246]
                                - cell [ref=e248]
                              - row [ref=e250]:
                                - cell [ref=e251]
                                - cell [ref=e253]
                                - cell [ref=e255]
                                - cell [ref=e257]
                    - generic [ref=e264] [cursor=pointer]:
                      - generic [ref=e265]:
                        - generic [ref=e266]: 
                        - generic [ref=e269]: "2.2"
                      - generic [ref=e270]:
                        - generic [ref=e272]:
                          - textbox "SignatureStep HEADER" [ref=e273]
                          - generic [ref=e275]: 
                        - generic [ref=e281]:
                          - paragraph [ref=e282]: Certification signature required
                          - paragraph
                          - generic [ref=e285]:
                            - textbox [ref=e289]:
                              - /placeholder: Sign
                            - textbox "Enter the Name" [disabled] [ref=e293]
                            - generic [ref=e297]:
                              - textbox:
                                - /placeholder: mm/dd/yyyy HH:MM
                            - textbox "User ID" [ref=e301]
                            - textbox "Enter Notes/Annotation" [ref=e305]
                  - generic [ref=e311]:
                    - generic [ref=e312]:
                      - img [ref=e314]
                      - generic [ref=e317]: Property Step
                    - generic [ref=e320]:
                      - generic [ref=e321]:
                        - generic [ref=e322]: Type
                        - generic:
                          - generic:
                            - generic: Step
                            - generic:
                              - img
                      - generic [ref=e323]:
                        - generic [ref=e324]: Step Type
                        - generic:
                          - generic:
                            - generic: Signature
                            - generic:
                              - img
                      - generic [ref=e325]:
                        - generic [ref=e326]: Signature Type
                        - generic [ref=e328] [cursor=pointer]:
                          - generic [ref=e329]: Select an option
                          - img [ref=e331]
                      - generic [ref=e333]:
                        - generic [ref=e334]: Applicable Point
                        - generic [ref=e336] [cursor=pointer]:
                          - generic [ref=e337]: Select an option
                          - img [ref=e339]
                      - generic [ref=e341]:
                        - generic [ref=e342]: Signature Prompt
                        - textbox "Signature Prompt" [ref=e343]
                      - generic [ref=e345] [cursor=pointer]:
                        - checkbox "Do not display Signature?" [ref=e346]
                        - generic [ref=e347]: Do not display Signature?
                      - generic [ref=e348]:
                        - generic [ref=e349]: Name Prompt
                        - textbox "Name Prompt" [ref=e350]
                      - generic [ref=e352] [cursor=pointer]:
                        - checkbox "Do not display Name?" [ref=e353]
                        - generic [ref=e354]: Do not display Name?
                      - generic [ref=e355]:
                        - generic [ref=e356]: Date/Time Prompt
                        - textbox "Date/Time Prompt" [ref=e357]
                      - generic [ref=e359]:
                        - generic [ref=e361] [cursor=pointer]:
                          - checkbox "Date?" [checked] [ref=e362]
                          - generic [ref=e363]: Date?
                        - generic [ref=e365] [cursor=pointer]:
                          - checkbox "Time?" [checked] [ref=e366]
                          - generic [ref=e367]: Time?
                      - generic [ref=e368]:
                        - generic [ref=e369]: Value
                        - generic [ref=e371] [cursor=pointer]:
                          - generic [ref=e372]: Entered
                          - img [ref=e374]
                      - generic [ref=e376]:
                        - generic [ref=e377]: User ID Prompt
                        - textbox "User ID Prompt" [ref=e378]
                      - generic [ref=e380] [cursor=pointer]:
                        - checkbox "Do not display User ID?" [ref=e381]
                        - generic [ref=e382]: Do not display User ID?
                      - generic [ref=e383]:
                        - generic [ref=e384]: Notes Prompt
                        - textbox "Notes Prompt" [ref=e385]
                      - generic [ref=e387] [cursor=pointer]:
                        - checkbox "Do not display Notes?" [ref=e388]
                        - generic [ref=e389]: Do not display Notes?
                      - generic [ref=e391]:
                        - text: Number
                        - paragraph: "2.2"
                      - generic [ref=e393]:
                        - text: UniqueID
                        - textbox [disabled] [ref=e394]: "52"
                      - button "Action Text" [ref=e396] [cursor=pointer]
                      - generic [ref=e398] [cursor=pointer]:
                        - checkbox "Is Critical?" [ref=e399]
                        - generic [ref=e400]: Is Critical?
                      - generic [ref=e402] [cursor=pointer]:
                        - checkbox "Required" [ref=e403]
                        - generic [ref=e404]: Required
                      - generic [ref=e406]:
                        - button "Applicability Rules" [ref=e408] [cursor=pointer]
                        - button "Role/Qualification" [ref=e410] [cursor=pointer]
```

# Test source

```ts
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
  58  |   await page.getByPlaceholder('Section HEADER').nth(1).click();
  59  | 
  60  |   // Skip Sticky Note section - button not clicking properly
  61  |   // await page.locator('button.dropbtn:has(app-action-icon.stickyNote)').click({ force: true });
  62  |   // await page.waitForSelector('textarea[name*="comment"], input[placeholder*="comment"], [role="textbox"]', { timeout: 5000 });
  63  |   // await page.getByRole('textbox', { name: 'Enter your comments here' }).click();
  64  |   // await page.getByRole('textbox', { name: 'Enter your comments here' }).fill('to proceed check the warnings');
  65  |   // await page.getByRole('button', { name: 'submit' }).click();
  66  |   // await page.locator('.fa.fa-times').first().click();
  67  |   
  68  |   // Click Sticky Note button in toolbar - using multiple selector attempts
  69  |   await page.getByPlaceholder('Section HEADER').nth(1).click();
  70  |   
  71  |   // Try different selectors for sticky note button
  72  |   const stickySelectors = [
  73  |     'button:has(app-action-icon.stickyNote)',
  74  |     'button.micon >> app-action-icon.stickyNote',
  75  |     'button >> app-action-icon[class*="sticky"]',
  76  |     '[class*="toolbar"] button:nth-child(6)', // Position-based fallback
  77  |   ];
  78  |   
  79  |   let clicked = false;
  80  |   for (const selector of stickySelectors) {
  81  |     try {
  82  |       await page.locator(selector).first().click({ timeout: 3000 });
  83  |       clicked = true;
  84  |       break;
  85  |     } catch (e) {
  86  |       continue;
  87  |     }
  88  |   }
  89  |   
  90  |   if (clicked) {
  91  |     await page.waitForTimeout(500);
  92  |     await page.locator('textarea[placeholder*="Enter your comments"], textarea[placeholder*="comments"]').fill('to proceed check the warnings');
  93  |     await page.locator('button.sbtn, button:has-text("submit"), button:has-text("Submit")').click();
  94  |     await page.locator('.fa-times, button:has-text("×")').first().click();
  95  |   }
  96  |   
  97  |   await page.locator('#step2').click();
  98  |   
  99  |   // Click Alert button and select Warning, Caution, Note
  100 |   const alertSelectors = [
  101 |     'button:has(app-action-icon.alert)',
  102 |     'button.micon >> app-action-icon.alert',
  103 |     'button >> app-action-icon[class*="alert"]',
  104 |   ];
  105 |   
  106 |   // Warning
  107 |   for (const selector of alertSelectors) {
  108 |     try {
  109 |       await page.locator(selector).first().click({ timeout: 2000 });
  110 |       await page.waitForTimeout(300);
  111 |       await page.getByRole('button', { name: 'Warning' }).click({ timeout: 2000 });
  112 |       break;
  113 |     } catch (e) { continue; }
  114 |   }
  115 |   
  116 |   // Caution
  117 |   for (const selector of alertSelectors) {
  118 |     try {
  119 |       await page.locator(selector).first().click({ timeout: 2000 });
  120 |       await page.waitForTimeout(300);
  121 |       await page.getByRole('button', { name: 'Caution' }).click({ timeout: 2000 });
  122 |       break;
  123 |     } catch (e) { continue; }
  124 |   }
  125 |   
  126 |   // Note
  127 |   for (const selector of alertSelectors) {
  128 |     try {
  129 |       await page.locator(selector).first().click({ timeout: 2000 });
  130 |       await page.waitForTimeout(300);
  131 |       await page.getByRole('button', { name: 'Note' }).click({ timeout: 2000 });
  132 |       break;
  133 |     } catch (e) { continue; }
  134 |   }
  135 |   
  136 |   await page.locator('#step2').click();
  137 |   await page.getByRole('button', { name: ' Action ' }).click();
  138 |   await page.locator('a').filter({ hasText: 'Add' }).click();
  139 |   await page.locator('a').filter({ hasText: 'Signature Step' }).click();
  140 |   await page.locator('#step2').click();
  141 |   await page.getByRole('button', { name: ' Action ' }).click();
> 142 |   await page.locator('a').filter({ hasText: 'Note' }).click();
      |                                                       ^ TimeoutError: locator.click: Timeout 30000ms exceeded.
  143 |   await page.locator('#note-17847913103150').click();
  144 |   await page.locator('#note-17847913103150').fill('');
  145 |   await page.locator('#note-17847913103150').click();
  146 |   await page.locator('#note-17847913103150').fill('cbp editor');
  147 |   await page.locator('#step1').click();
  148 |   await page.locator('div:nth-child(12) > button').click();
  149 |   await page.locator('.buttns.w-auto').first().click();
  150 |   await page.getByRole('button', { name: 'Choose File' }).setInputFiles(['1.jpg', '2025-03-18_092834.png', 'DAy.jpg', 'DG.png.png', 'girl-with-red-hat-BBZDOHhYU2s-unsplash.jpg', 'Greenary.jpg', 'Header Logo7257437.png', '-icon-logo.png', 'Image.jpg', 'istockphoto-1152614033-612x612.jpg', 'jpeg.jfif', 'jpeg1.jfif', 'jpeg2.jfif', 'jpeg3.jfif', 'jpeg4.jpg', 'jpeg5.jpg', 'jpeg6.jfif', 'jpeg7.jpg', 'jpeg8.jpg', 'jpeg9.jpeg', 'JPG.jpg', 'Keep Going.jpg', 'Motivational-quotes-image-for-work-768x432.jpg.jpg', 'PNG.png', 'PNG2.jfif', 'River.jpg', 'Robot.jpg', 'Soft.jpg', 'software.jpg', 'Success.jpg', 'Sunrise.jpg', 'Tata.jpg', 'Test.jpeg', 'tiger jpeg.jfif', 'Tree.jpg', 'Water.jpg', 'you did it!.jpg']);
  151 |   await page.locator('#step1').click();
  152 |   await page.locator('div:nth-child(12) > button').click();
  153 |   await page.locator('.d-flex > button:nth-child(3)').click();
  154 |   await page.locator('#fileUploadMedia').setInputFiles('DG.png.png');
  155 |   await page.getByRole('combobox').selectOption('center');
  156 |   await page.locator('.btn-trans.btn.btn-icon.ng-star-inserted').click();
  157 |   await page.getByRole('textbox').nth(1).fill('dataglance');
  158 |   await page.locator('.ng-resizable-handle').click();
  159 |   await page.locator('#scrollSection3 #stop_draging_id').click();
  160 |   await page.locator('.fa.fa-edit').click();
  161 |   await page.locator('#cbp-editor').click();
  162 |   await page.locator('#cbp-editor').fill('Enter text properly');
  163 |   await page.getByRole('textbox', { name: 'Action Step HEADER' }).click();
  164 |   await page.getByRole('button', { name: 'Basic' }).click();
  165 |   await page.getByRole('button', { name: 'Basic' }).click();
  166 |   await page.getByText('Signature Step').nth(2).click();
  167 | });
  168 | 
```