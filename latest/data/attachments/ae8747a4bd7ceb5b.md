# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: cbp-editor\testing.spec.ts >> creating basic cbp
- Location: tests\cbp-editor\testing.spec.ts:8:5

# Error details

```
Error: locator.click: Error: strict mode violation: locator('.dg-select-option').filter({ hasText: 'Text' }) resolved to 2 elements:
    1) <div _ngcontent-ng-c1246892924="" class="dg-select-option ng-star-inserted">…</div> aka locator('#tablePropertie').getByText('Text', { exact: true })
    2) <div _ngcontent-ng-c1246892924="" class="dg-select-option ng-star-inserted">…</div> aka locator('#tablePropertie').getByText('TextArea')

Call log:
  - waiting for locator('.dg-select-option').filter({ hasText: 'Text' })

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
                  - text:                                                                    
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
                        - heading "Basic" [level=5] [ref=e103]:
                          - button "Basic" [ref=e104] [cursor=pointer]
                        - generic [ref=e105]:
                          - heading "Data Entry" [level=5] [ref=e107]:
                            - button "Data Entry" [ref=e108] [cursor=pointer]
                          - generic [ref=e110]:
                            - generic [ref=e111]:
                              - generic [ref=e112]: 
                              - text: Text
                              - generic [ref=e114]: 
                            - generic [ref=e115]:
                              - generic [ref=e116]: 
                              - text: TextArea
                              - generic [ref=e118]: 
                            - generic [ref=e119]:
                              - generic [ref=e120]: 
                              - text: Number
                              - generic [ref=e122]: 
                            - generic [ref=e123]:
                              - generic [ref=e124]: 
                              - text: Date
                              - generic [ref=e126]: 
                            - generic [ref=e127]:
                              - generic [ref=e128]: 
                              - text: Boolean
                              - generic [ref=e130]: 
                            - generic [ref=e131]:
                              - generic [ref=e132]: 
                              - text: Radio Button
                              - generic [ref=e134]: 
                            - generic:
                              - generic: 
                              - text: Check Box Group
                              - generic:
                                - generic: 
                            - generic [ref=e135]:
                              - generic [ref=e136]: 
                              - text: Check Box
                              - generic [ref=e138]: 
                            - generic [ref=e139]:
                              - generic [ref=e140]: 
                              - text: Button
                              - generic [ref=e142]: 
                            - generic [ref=e143]:
                              - generic [ref=e144]: 
                              - text: Drop Down
                              - generic [ref=e146]: 
                            - generic [ref=e147]:
                              - generic [ref=e148]: 
                              - text: Table
                              - generic [ref=e150]: 
                        - heading "Reference/Link" [level=5] [ref=e153]:
                          - button "Reference/Link" [ref=e154] [cursor=pointer]
                        - heading "Verification" [level=5] [ref=e157]:
                          - button "Verification" [ref=e158] [cursor=pointer]
                    - text:                                            
                  - generic [ref=e162]:
                    - generic [ref=e166] [cursor=pointer]:
                      - generic [ref=e167]:
                        - img [ref=e168]:
                          - img [ref=e169]
                        - generic [ref=e173]: "1.0"
                      - generic [ref=e174]:
                        - textbox "Section HEADER" [ref=e177]
                        - generic [ref=e186]:
                          - generic [ref=e187]:
                            - img [ref=e189]
                            - heading "Warning" [level=4] [ref=e197]
                            - img [ref=e199]
                          - generic [ref=e209]:
                            - textbox "Enter your cause" [ref=e212]: Warning cause
                            - textbox "Enter your effect" [ref=e215]: Warning effect
                        - generic [ref=e224]:
                          - generic [ref=e225]:
                            - img [ref=e227]
                            - heading "Caution" [level=4] [ref=e230]
                            - img [ref=e232]
                          - generic [ref=e237]:
                            - textbox "Enter your cause" [ref=e240]: caution cause
                            - textbox "Enter your effect" [ref=e243]: caution effect
                        - generic [ref=e252]:
                          - generic [ref=e253]:
                            - img [ref=e255]
                            - heading "Alara" [level=4] [ref=e272]
                            - img [ref=e274]
                          - textbox "Enter your note" [ref=e296]: This is a note message
                        - textbox "Enter the Label" [ref=e305]: This is a label message
                        - generic [ref=e320]:
                          - text:  
                          - img "img" [ref=e323]
                          - paragraph [ref=e326]:
                            - generic [ref=e328]: 
                        - generic [ref=e340]:
                          - generic [ref=e343]:
                            - text:  
                            - img "-icon-logo.png" [ref=e345]
                            - paragraph [ref=e347]:
                              - generic [ref=e349]: 
                          - generic [ref=e352]:
                            - text:  
                            - img "1.jpg" [ref=e354]
                            - paragraph [ref=e356]:
                              - generic [ref=e358]: 
                          - generic [ref=e361]:
                            - text:  
                            - img "2025-03-18_092834.png" [ref=e363]
                            - paragraph [ref=e365]:
                              - generic [ref=e367]: 
                          - generic [ref=e370]:
                            - text:  
                            - img "DAy.jpg" [ref=e372]
                            - paragraph [ref=e374]:
                              - generic [ref=e376]: 
                          - generic [ref=e379]:
                            - text:  
                            - img "DG.png" [ref=e381]
                            - paragraph [ref=e383]:
                              - generic [ref=e385]: 
                          - generic [ref=e388]:
                            - text:  
                            - img "girl-with-red-hat-BBZDOHhYU2s-unsplash.jpg" [ref=e390]
                            - paragraph [ref=e392]:
                              - generic [ref=e394]: 
                          - generic [ref=e397]:
                            - text:  
                            - img "Greenary.jpg" [ref=e399]
                            - paragraph [ref=e401]:
                              - generic [ref=e403]: 
                          - generic [ref=e406]:
                            - text:  
                            - img "Header Logo7257437.png" [ref=e408]
                            - paragraph [ref=e410]:
                              - generic [ref=e412]: 
                          - generic [ref=e415]:
                            - text:  
                            - img "Image.jpg" [ref=e417]
                            - paragraph [ref=e419]:
                              - generic [ref=e421]: 
                          - generic [ref=e424]:
                            - text:  
                            - img "istockphoto-1152614033-612x612.jpg" [ref=e426]
                            - paragraph [ref=e428]:
                              - generic [ref=e430]: 
                          - generic [ref=e433]:
                            - text:  
                            - img "jpeg.jfif" [ref=e435]
                            - paragraph [ref=e437]:
                              - generic [ref=e439]: 
                          - generic [ref=e442]:
                            - text:  
                            - img "jpeg1.jfif" [ref=e444]
                            - paragraph [ref=e446]:
                              - generic [ref=e448]: 
                          - generic [ref=e451]:
                            - text:  
                            - img "jpeg2.jfif" [ref=e453]
                            - paragraph [ref=e455]:
                              - generic [ref=e457]: 
                          - generic [ref=e460]:
                            - text:  
                            - img "jpeg3.jfif" [ref=e462]
                            - paragraph [ref=e464]:
                              - generic [ref=e466]: 
                          - generic [ref=e469]:
                            - text:  
                            - img "jpeg4.jpg" [ref=e471]
                            - paragraph [ref=e473]:
                              - generic [ref=e475]: 
                          - generic [ref=e478]:
                            - text:  
                            - img "jpeg5.jpg" [ref=e480]
                            - paragraph [ref=e482]:
                              - generic [ref=e484]: 
                          - generic [ref=e487]:
                            - text:  
                            - img "jpeg6.jfif" [ref=e489]
                            - paragraph [ref=e491]:
                              - generic [ref=e493]: 
                          - generic [ref=e496]:
                            - text:  
                            - img "jpeg7.jpg" [ref=e498]
                            - paragraph [ref=e500]:
                              - generic [ref=e502]: 
                          - generic [ref=e505]:
                            - text:  
                            - img "jpeg8.jpg" [ref=e507]
                            - paragraph [ref=e509]:
                              - generic [ref=e511]: 
                          - generic [ref=e514]:
                            - text:  
                            - img "jpeg9.jpeg" [ref=e516]
                            - paragraph [ref=e518]:
                              - generic [ref=e520]: 
                          - generic [ref=e523]:
                            - text:  
                            - img "JPG.jpg" [ref=e525]
                            - paragraph [ref=e527]:
                              - generic [ref=e529]: 
                          - generic [ref=e532]:
                            - text:  
                            - img "Keep Going.jpg" [ref=e534]
                            - paragraph [ref=e536]:
                              - generic [ref=e538]: 
                          - generic [ref=e541]:
                            - text:  
                            - img "Motivational-quotes-image-for-work-768x432.jpg.jpg" [ref=e543]
                            - paragraph [ref=e545]:
                              - generic [ref=e547]: 
                          - generic [ref=e550]:
                            - text:  
                            - img "PNG.png" [ref=e552]
                            - paragraph [ref=e554]:
                              - generic [ref=e556]: 
                          - generic [ref=e559]:
                            - text:  
                            - img "PNG2.jfif" [ref=e561]
                            - paragraph [ref=e563]:
                              - generic [ref=e565]: 
                          - generic [ref=e568]:
                            - text:  
                            - img "River.jpg" [ref=e570]
                            - paragraph [ref=e572]:
                              - generic [ref=e574]: 
                          - generic [ref=e577]:
                            - text:  
                            - img "Robot.jpg" [ref=e579]
                            - paragraph [ref=e581]:
                              - generic [ref=e583]: 
                          - generic [ref=e586]:
                            - text:  
                            - img "Soft.jpg" [ref=e588]
                            - paragraph [ref=e590]:
                              - generic [ref=e592]: 
                          - generic [ref=e595]:
                            - text:  
                            - img "software.jpg" [ref=e597]
                            - paragraph [ref=e599]:
                              - generic [ref=e601]: 
                          - generic [ref=e604]:
                            - text:  
                            - img "Success.jpg" [ref=e606]
                            - paragraph [ref=e608]:
                              - generic [ref=e610]: 
                          - generic [ref=e613]:
                            - text:  
                            - img "Sunrise.jpg" [ref=e615]
                            - paragraph [ref=e617]:
                              - generic [ref=e619]: 
                          - generic [ref=e622]:
                            - text:  
                            - img "Tata.jpg" [ref=e624]
                            - paragraph [ref=e626]:
                              - generic [ref=e628]: 
                          - generic [ref=e631]:
                            - text:  
                            - img "Test.jpeg" [ref=e633]
                            - paragraph [ref=e635]:
                              - generic [ref=e637]: 
                          - generic [ref=e640]:
                            - text:  
                            - img "tiger jpeg.jfif" [ref=e642]
                            - paragraph [ref=e644]:
                              - generic [ref=e646]: 
                          - generic [ref=e649]:
                            - text:  
                            - img "Tree.jpg" [ref=e651]
                            - paragraph [ref=e653]:
                              - generic [ref=e655]: 
                          - generic [ref=e658]:
                            - text:  
                            - img "Water.jpg" [ref=e660]
                            - paragraph [ref=e662]:
                              - generic [ref=e664]: 
                          - generic [ref=e667]:
                            - text:  
                            - img "you did it!.jpg" [ref=e669]
                            - paragraph [ref=e671]:
                              - generic [ref=e673]: 
                          - generic [ref=e675]:
                            - generic [ref=e676]:
                              - generic [ref=e677]: 
                              - text: Add Media
                            - button "Choose File" [ref=e678]
                    - generic [ref=e680]:
                      - generic [ref=e684] [cursor=pointer]:
                        - generic [ref=e685]:
                          - img [ref=e686]:
                            - img [ref=e687]
                          - generic [ref=e692]: "1.1"
                        - generic [ref=e693]:
                          - textbox "Sub Section HEADER" [ref=e696]
                          - table [ref=e705]:
                            - rowgroup [ref=e706]:
                              - row "Column1 Column2 Column3 Column4" [ref=e707]:
                                - columnheader "Column1" [ref=e708]:
                                  - generic [ref=e709]: Column1
                                - columnheader "Column2" [ref=e711]:
                                  - generic [ref=e712]: Column2
                                - columnheader "Column3" [ref=e714]:
                                  - generic [ref=e715]: Column3
                                - columnheader "Column4" [ref=e717]:
                                  - generic [ref=e718]: Column4
                            - rowgroup [ref=e719]:
                              - row [ref=e720]:
                                - cell [ref=e721]
                                - cell [ref=e723]
                                - cell [ref=e725]
                                - cell [ref=e727]
                              - row [ref=e729]:
                                - cell [ref=e730]
                                - cell [ref=e732]
                                - cell [ref=e734]
                                - cell [ref=e736]
                              - row [ref=e738]:
                                - cell [ref=e739]
                                - cell [ref=e741]
                                - cell [ref=e743]
                                - cell [ref=e745]
                              - row [ref=e747]:
                                - cell [ref=e748]
                                - cell [ref=e750]
                                - cell [ref=e752]
                                - cell [ref=e754]
                              - row [ref=e756]:
                                - cell [ref=e757]
                                - cell [ref=e759]
                                - cell [ref=e761]
                                - cell [ref=e763]
                      - generic [ref=e770] [cursor=pointer]:
                        - generic [ref=e771]:
                          - generic [ref=e772]: 
                          - generic [ref=e775]: 1.1.1
                        - generic [ref=e776]:
                          - textbox "Action Step HEADER" [ref=e779]: This is an action step header
                          - generic [ref=e789]:
                            - textbox "Please Enter the Text" [ref=e794]: This is a text data entry
                            - generic [ref=e796]: Enter The Text
                          - textbox "text..." [ref=e805]
                          - generic [ref=e812]:
                            - textbox "Please Enter a Date" [ref=e817]:
                              - /placeholder: "Please Enter a Date "
                              - text: Enter a date
                            - generic [ref=e819]: mm/dd/yyyy
                          - generic [ref=e826]:
                            - textbox "Please Enter the Boolean" [ref=e831]
                            - generic [ref=e833]:
                              - generic [ref=e834]:
                                - radio "Yes" [disabled] [ref=e835]
                                - text: "Yes"
                              - generic [ref=e836]:
                                - radio "No" [disabled] [ref=e837]
                                - text: "No"
                          - generic [ref=e846]:
                            - textbox "Enter Question" [ref=e851]: Select one of the option
                            - generic [ref=e852]:
                              - generic [ref=e854]:
                                - radio [ref=e855]
                                - generic [ref=e856]: option 1
                              - generic [ref=e858]:
                                - radio [ref=e859]
                                - generic [ref=e860]: option 2
                              - generic [ref=e862]:
                                - radio [ref=e863]
                                - generic [ref=e864]: option 3
                  - generic [ref=e870]:
                    - generic [ref=e871]:
                      - img [ref=e873]
                      - generic [ref=e876]: Property Table
                    - generic [ref=e879]:
                      - generic [ref=e880]:
                        - generic [ref=e881]: Data Type
                        - textbox [ref=e882]: Table
                      - generic [ref=e883]:
                        - generic [ref=e884]: Table Name
                        - textbox "Table Name" [ref=e885]: Table54
                      - generic [ref=e887]:
                        - text: UniqueID
                        - textbox [disabled] [ref=e888]: "53"
                      - generic [ref=e890]:
                        - button "Table Rule" [ref=e892] [cursor=pointer]
                        - generic [ref=e895]:
                          - generic [ref=e896] [cursor=pointer]: Exclude Rows
                          - spinbutton [ref=e897]: "0"
  - dialog [active] [ref=e899]:
    - document:
      - generic [ref=e901]:
        - generic [ref=e903]:
          - heading "Table Property" [level=6] [ref=e904]
          - generic "Close" [ref=e905] [cursor=pointer]:
            - generic [ref=e906]: ×
        - generic [ref=e907]:
          - generic [ref=e908]:
            - generic [ref=e909]: Section
            - paragraph [ref=e910]: "1.1"
          - generic [ref=e911]:
            - list [ref=e912]:
              - listitem [ref=e913]:
                - generic [ref=e914] [cursor=pointer]:
                  - generic [ref=e915]: 
                  - text: Table
              - listitem [ref=e916]:
                - generic [ref=e917] [cursor=pointer]:
                  - generic [ref=e918]: 
                  - text: Column
            - generic [ref=e920]:
              - table [ref=e922]:
                - rowgroup [ref=e923]:
                  - row "Position Title Column Size(%) Data Type Field Name" [ref=e924]:
                    - columnheader "Position" [ref=e925]
                    - columnheader "Title" [ref=e926]
                    - columnheader "Column Size(%)" [ref=e927]
                    - columnheader "Data Type" [ref=e928]
                    - columnheader "Field Name" [ref=e929]
                - rowgroup [ref=e930]:
                  - row "1 Column1 25 Column1" [ref=e931] [cursor=pointer]:
                    - cell "1" [ref=e932]
                    - cell "Column1" [ref=e933]
                    - cell "25" [ref=e934]
                    - cell [ref=e935]
                    - cell "Column1" [ref=e936]
                  - row "2 Column2 25 Column2" [ref=e937] [cursor=pointer]:
                    - cell "2" [ref=e938]
                    - cell "Column2" [ref=e939]
                    - cell "25" [ref=e940]
                    - cell [ref=e941]
                    - cell "Column2" [ref=e942]
                  - row "3 Column3 25 Column3" [ref=e943] [cursor=pointer]:
                    - cell "3" [ref=e944]
                    - cell "Column3" [ref=e945]
                    - cell "25" [ref=e946]
                    - cell [ref=e947]
                    - cell "Column3" [ref=e948]
                  - row "4 Column4 25 Column4" [ref=e949] [cursor=pointer]:
                    - cell "4" [ref=e950]
                    - cell "Column4" [ref=e951]
                    - cell "25" [ref=e952]
                    - cell [ref=e953]
                    - cell "Column4" [ref=e954]
              - generic [ref=e956]:
                - generic [ref=e959]:
                  - heading "Column Property" [level=2] [ref=e961]
                  - generic [ref=e963]:
                    - generic [ref=e964] [cursor=pointer]: 
                    - generic: 
                    - generic [ref=e965] [cursor=pointer]: 
                    - generic [ref=e966] [cursor=pointer]: 
                - generic [ref=e967]:
                  - generic [ref=e970]:
                    - generic [ref=e971]: Position
                    - textbox [ref=e972]: "1"
                  - generic [ref=e974]:
                    - generic [ref=e975]:
                      - generic [ref=e976]: Title
                      - textbox [ref=e977]: Column1
                    - generic [ref=e978]:
                      - generic [ref=e979]: Column Size(%)
                      - spinbutton [ref=e980]: "25"
                  - generic [ref=e983]:
                    - generic [ref=e984]: Data Type
                    - generic [ref=e986]:
                      - generic [ref=e987] [cursor=pointer]:
                        - generic [ref=e988]: Select an option
                        - img [ref=e990]
                      - generic [ref=e993]:
                        - generic [ref=e994] [cursor=pointer]: Text
                        - generic [ref=e995] [cursor=pointer]: TextArea
                        - generic [ref=e996] [cursor=pointer]: Numeric
                        - generic [ref=e997] [cursor=pointer]: Date
                        - generic [ref=e998] [cursor=pointer]: Checkbox
                        - generic [ref=e999] [cursor=pointer]: Dropdown
                        - generic [ref=e1000] [cursor=pointer]: Boolean
                        - generic [ref=e1001] [cursor=pointer]: Para
                        - generic [ref=e1002] [cursor=pointer]: Label
                        - generic [ref=e1003] [cursor=pointer]: Button
                  - generic [ref=e1006]:
                    - generic [ref=e1007]: Field Name
                    - textbox [ref=e1008]: Column1
        - generic [ref=e1009]:
          - button "Reset" [disabled]
          - button "Ok" [ref=e1010] [cursor=pointer]
          - button "Cancel" [ref=e1011] [cursor=pointer]
```

# Test source

```ts
  111 | 
  112 | // Wait for file chooser while dragging
  113 | const [fileChooser] = await Promise.all([
  114 |     page.waitForEvent('filechooser'),
  115 |     mediaSingle.dragTo(sectionHeader)
  116 | ]);
  117 | 
  118 | // Upload image
  119 | 
  120 | await fileChooser.setFiles(imagePath);
  121 | 
  122 | await page.waitForTimeout(500); // Wait for the section to be selected
  123 | 
  124 | await page.getByRole('textbox', { name: 'Section HEADER' }).click();
  125 | // Media Gallery upload
  126 | const mediaGallery = page
  127 |     .getByText('Media Gallery', { exact: true })
  128 |     .nth(1);
  129 | 
  130 | await mediaGallery.dragTo(sectionHeader);
  131 | await page.mouse.wheel(0, 900);
  132 | const fileInput = page.locator('#files');
  133 | 
  134 | await expect(fileInput).toBeVisible();
  135 | 
  136 | await FileUploadHelper.uploadAllImages(fileInput);
  137 | 
  138 | 
  139 | await page.waitForTimeout(1000);
  140 | await page.getByRole('textbox', { name: 'Section HEADER' }).click();
  141 | 
  142 | await page.getByRole('button', { name: 'Basic' }).nth(0).click();
  143 |  await page.getByText('Sub Section').nth(2).click();
  144 | await page.getByRole('textbox', { name: 'Sub Section HEADER' }).click();
  145 | await page.getByText('Action Step').nth(1).click();
  146 | 
  147 | page.getByPlaceholder('Action Step HEADER', { exact: true }).click();
  148 | await page.getByPlaceholder('Action Step HEADER', { exact: true }).fill('This is an action step header');
  149 | await page.getByRole('button', { name: 'Data Entry' }).nth(0).click();
  150 | await page.waitForTimeout(500);
  151 | const text_dataentry = page.getByText('Text', { exact: true }).nth(1);
  152 | const target_actionstep = page.getByPlaceholder('Action Step HEADER', { exact: true });
  153 | await expect(text_dataentry).toBeVisible();
  154 | await text_dataentry.scrollIntoViewIfNeeded();
  155 | await text_dataentry.dragTo(target_actionstep);
  156 | await page.waitForTimeout(500);
  157 | await page.getByPlaceholder('Please Enter the Text').fill('This is a text data entry');
  158 | page.getByPlaceholder('Action Step HEADER', { exact: true }).click();
  159 | const textarea_dataentry = page.getByText('TextArea', { exact: true }).nth(1);
  160 | await expect(textarea_dataentry).toBeVisible();
  161 | await textarea_dataentry.scrollIntoViewIfNeeded();
  162 | await textarea_dataentry.dragTo(target_actionstep);
  163 | //await page.getByRole('textbox', { name: 'text...' }).fill('This is a text area data entry');
  164 | await page.mouse.wheel(0, 300);
  165 | //await page.getByRole('textbox', { name: 'Enter your text' }).fill('This is a text data entry');
  166 | await page.waitForTimeout(1000);
  167 | page.getByPlaceholder('Action Step HEADER', { exact: true }).click();
  168 | const date_dataentry = page.getByText('Date', { exact: true }).nth(1);
  169 | await expect(date_dataentry).toBeVisible();
  170 | await date_dataentry.scrollIntoViewIfNeeded();
  171 | await date_dataentry.dragTo(target_actionstep); 
  172 | await page.getByRole('textbox', { name: 'Please Enter a Date' }).fill('Enter a date');
  173 | await page.waitForTimeout(1000);
  174 | await page.mouse.wheel(0, 100);
  175 | page.getByPlaceholder('Action Step HEADER', { exact: true }).click();
  176 | const boolean_dataentry = page.getByText('Boolean', { exact: true }).nth(1);
  177 | await expect(boolean_dataentry).toBeVisible();
  178 | await boolean_dataentry.scrollIntoViewIfNeeded();
  179 | await boolean_dataentry.dragTo(target_actionstep);
  180 | await page.waitForTimeout(1000);
  181 | await page.mouse.wheel(0, 100);
  182 | page.getByPlaceholder('Action Step HEADER', { exact: true }).click();
  183 | const radio_button_dataentry = page.getByText('Radio Button').nth(1);
  184 | await expect(radio_button_dataentry).toBeVisible();
  185 | await radio_button_dataentry.scrollIntoViewIfNeeded();
  186 | await radio_button_dataentry.dragTo(target_actionstep);
  187 | await page.waitForTimeout(1000);
  188 | await page.mouse.wheel(0, 100);
  189 | 
  190 | await page.getByRole('textbox', { name: 'Sub Section HEADER' }).click();
  191 | //await page.getByRole('button', { name: 'Data Entry' }).nth(0).click();
  192 | const table_dataentry = page.getByText('Table', { exact: true }).nth(1);
  193 | const target_subsection = page.getByRole('textbox', { name: 'Sub Section HEADER' });
  194 | await expect(table_dataentry).toBeVisible();
  195 | await table_dataentry.scrollIntoViewIfNeeded();
  196 | await table_dataentry.dragTo(target_subsection);
  197 | await page.waitForTimeout(1000);
  198 | await page.getByRole('spinbutton').first().click();
  199 | await page.getByRole('spinbutton').first().fill('4');
  200 | await page.getByRole('spinbutton').nth(1).click();
  201 | await page.getByRole('spinbutton').nth(1).fill('5');
  202 | await page.getByRole('button', { name: 'Ok' }).click();
  203 | await page.getByText('Column', { exact: true }).click();
  204 | await page.locator('tr.cdk-drag.e-point.selected-table.ng-star-inserted').locator('td').nth(3).click();
  205 | await page.getByText('Select an option', { exact: true }).first().click();
  206 | 
  207 | await page.locator('.dg-select-option').first().waitFor();
  208 | 
  209 | await page.locator('.dg-select-option', {
  210 |     hasText: 'Text'
> 211 | }).click();
      |    ^ Error: locator.click: Error: strict mode violation: locator('.dg-select-option').filter({ hasText: 'Text' }) resolved to 2 elements:
  212 | 
  213 | await page.getByRole('button', { name: 'Ok' }).click();
  214 | 
  215 | await page.waitForTimeout(1000);
  216 | 
  217 | });
```