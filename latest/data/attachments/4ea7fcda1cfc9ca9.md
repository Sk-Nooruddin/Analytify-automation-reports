# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: auth.setup.ts >> Authenticate User
- Location: tests\auth.setup.ts:8:6

# Error details

```
Error: page.goto: net::ERR_CONNECTION_TIMED_OUT at http://34.220.72.148/emediaNew/login
Call log:
  - navigating to "http://34.220.72.148/emediaNew/login", waiting until "load"

```

# Page snapshot

```yaml
- generic [ref=e3]:
  - generic [ref=e6]:
    - heading "This site can’t be reached" [level=1] [ref=e7]
    - paragraph [ref=e8]:
      - strong [ref=e9]: 34.220.72.148
      - text: took too long to respond.
    - generic [ref=e10]:
      - paragraph [ref=e11]: "Try:"
      - list [ref=e12]:
        - listitem [ref=e13]: Checking the connection
        - listitem [ref=e14]:
          - link "Checking the proxy and the firewall" [ref=e15] [cursor=pointer]:
            - /url: "#buttons"
        - listitem [ref=e16]:
          - link "Running Windows Network Diagnostics" [ref=e17] [cursor=pointer]:
            - /url: javascript:diagnoseErrors()
    - generic [ref=e18]: ERR_CONNECTION_TIMED_OUT
  - generic [ref=e19]:
    - button "Reload" [ref=e21] [cursor=pointer]
    - button "Details" [ref=e22] [cursor=pointer]
```

# Test source

```ts
  1   | import { expect, Page } from "@playwright/test";
  2   | 
  3   | import { LoginLocator } from "../locators/LoginLocator";
  4   | import { Environment } from "../config/Environment";
  5   | 
  6   | export class LoginPage {
  7   | 
  8   |     readonly locator: LoginLocator;
  9   | 
  10  |     constructor(private readonly page: Page) {
  11  | 
  12  |         this.locator = new LoginLocator(page);
  13  | 
  14  |     }
  15  | 
  16  |     async navigate(): Promise<void> {
  17  | 
> 18  |         await this.page.goto(Environment.baseUrl);
      |                         ^ Error: page.goto: net::ERR_CONNECTION_TIMED_OUT at http://34.220.72.148/emediaNew/login
  19  | 
  20  |     }
  21  | 
  22  |     async login(
  23  |         username: string,
  24  |         password: string
  25  |     ): Promise<void> {
  26  | 
  27  |         await this.locator.userName.fill(username);
  28  | 
  29  |         await this.locator.password.fill(password);
  30  | 
  31  |         await this.locator.loginButton.click();
  32  | 
  33  |     }
  34  | 
  35  |     async verifySuccessfulLogin(): Promise<void> {
  36  | 
  37  |         await expect(
  38  |             this.locator.welcomeMessage
  39  |         ).toBeVisible();
  40  | 
  41  |     }
  42  | 
  43  |     async closeWelcomePopup(): Promise<void> {
  44  | 
  45  |         if (
  46  |             await this.locator.closePopupButton.isVisible()
  47  |         ) {
  48  | 
  49  |             await this.locator.closePopupButton.click();
  50  | 
  51  |         }
  52  | 
  53  |     }
  54  | async verifyLoginPageDisplayed(): Promise<void> {
  55  | 
  56  |     await expect(this.locator.userName).toBeVisible();
  57  | 
  58  |     await expect(this.locator.password).toBeVisible();
  59  | 
  60  |     await expect(this.locator.loginButton).toBeVisible();
  61  | 
  62  | }
  63  | async verifyLoginFailure(): Promise<void> {
  64  | 
  65  |     await expect(
  66  |         this.locator.errorPopup
  67  |     ).toBeVisible({timeout: 5000});
  68  | 
  69  | }
  70  | async verifyErrorMessage(
  71  |     expectedMessage: string
  72  | ): Promise<void> {
  73  | 
  74  |     await expect(
  75  |         this.locator.errorPopupMessage
  76  |     ).toContainText(expectedMessage);
  77  | 
  78  | }
  79  | async closeErrorPopup(): Promise<void> {
  80  | 
  81  |     if (
  82  |         await this.locator.errorPopupCancelButton.isVisible()
  83  |     ) {
  84  | 
  85  |         await this.locator.errorPopupCancelButton.click();
  86  | 
  87  |     }
  88  | 
  89  | }
  90  | async enableRememberMe(): Promise<void> {
  91  | 
  92  |     if (!(await this.locator.rememberMe.isChecked())) {
  93  | 
  94  |         await this.locator.rememberMe.check();
  95  | 
  96  |     }
  97  | 
  98  | }
  99  | 
  100 | async verifyRememberMeChecked(): Promise<void> {
  101 | 
  102 |     await expect(
  103 |         this.locator.rememberMe
  104 |     ).toBeChecked();
  105 | 
  106 | }
  107 | }
```