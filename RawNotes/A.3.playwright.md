Playwright automation testing from scratch with framework

Reliable end to end testing

Playwright's Auto wait capability (No sync issues)

Cross Browser compatibility

Multiplatform support

Multilingual flexibility

PlayWright's Advanced Feature

Auto screenshot and video (tracing and dubugging)

Network interception

Browser context management (use cookies)

Codegen Tool (test code by just recording actions)

Const (test) = require('@playwright/test');

test('name' function()()); //syntax for test cases

Styles

javascript is asynchronous thus we have to spcifically mention to follow the flow to do that we need

test ('name', async (browser) =>

{

});

Fixture-browser is a global fixture, to use browser we need to send browser fixture in the function

we wrap it using {} to tell pw that it is a fixture otherwise it will take it as a normal variable

test ('name', async ({browser)) =>

{

//create instance of browser-plugins/cookies

const context await browser.newContext():

//newContext()-we can use this to inject cookies and proxy

const page await context.newPage(); //context and page need not to be done if no cookies needs to installed

await page.goto("url"):

//browser information is made in playwright.config.json

const {test)= require("@playwright/test");

test('name', async ({browser, page)) => {

await page.goto("url"); });

playwright.config.js

import {defineConfig, devices) from '@playwright/test

export default defineConfig((

testDir: /tests',

use: {

J.

1);

import (defineConfig, devices) from @playwright/test';

export default defineConfig({

testDir:/tests',

timeout: 40*1000.

expect: {

timeout: 40*1000,

reporter: 'html',

use: {

browserName: 'chromium’

)}})}}




npx-nox, is the path which will point to the path of node modules,

test in same file will run sequentientially.

test files will run parallelly

npx playwright test

Dx, playwright test-headed

is the omd used to run playwright tests

test.only!) //only this will be runned

const {test, expect) require(');

test('name', async ({page))=>

});

to use headed mode

await page.goto("google.com");

console.log(await page.title());

await expect(page).toHaveTitle("Google");


for safari it is webkit

use: (headless: false)

Gas, selector, xpath

selectors

Rage.jocator():

Css selector

if id is present tagname#id or #id

if class attribute-tangname.class or.class

any attribute -> [attribute 'value'], [attribute 'partialvalue'l

text-text=”


await page locator("").fill("learning");

await page locator(").click():

//type is deprecated

console.log(await page, locator("[style='block"]").textContent()):

await expect(page.locator().toContainText('abcd'));

const userName = page locator('#usemaem'):

await userName.fill("");

//clears the already entered variable

await userName.fill("abcd");

await page.locator("").nth(0).textContent():

all elements

const allTextinWebElements, await web.Element.allTextContents();

//allTextContents doesn't have that auto wait so some other code for that should be used before this code.

Waiting till all API call's are made

await page.waitForLoadStatel networkidle");

await page, locator(".card-body b").first().waitFor();

//to wait for allTextContent

Radio Button and DropDowns

Select Drop Downs-

const dropdown-page.locator("select.form-control");

await dropdown.selectOption("consult");

await page.pause(); //playwright inspector

Radio Button-

await page locator!" radiotextsty").last().click();

await page.locator("#okayBtn").click();

await page.locator("radiotext").last().jsChecked0):

await expect(page.locator("radiotext").last()).toBeChecked():

.uncheck():

expect().toße Falay();

expect().toBeTruthy():

toHaveAttribute("class", "atributeName"):

Window Handling

test('child window', async ((browser)))

1

Styles

const context await browser.newConent():

const page await context.newPage():

await page goto("");

const documentLink page.locater("");

// pending, rejected, fulfilled

const [new page] = Promise.all

context.waitForEvent('page'),

//use comma

//listen for any page is opened

documentLink.click().

//listen first then execute

1

await newPage.locator("").click():

});

npx, playwright test-debug

playwright inspector will run one by one line of code

in config file

use: {

screenshot:

'on',

}

trace: 'on’


Special Locators

Get by label-

await page.getByLabel("text which that label tag has").click(); //label tag in html,

await page.getBylabel("gender").selectOption("female"); //if the html has select tag init

Get by role

Get by placeholder

DBX playwright test-ui

Sheryala Sai Keerthi's session.

In typeScript in regress website

import (test, expect) from "@playwright/test";

test("API Testing", async ((request)) => {

const response request.get("https:url");

console.log(await response.status());

console.log(await response.ison());

});

to run, in terminal type gpx playwright test

Assertions

expect(await response.status())-toße(200);

expect ((await response.ison()) data.first, name)-toBe("Janet");

Back to Udemy Course.

Locators,

await page.getByPlaceholder("Password").fill("abc123");

await page.getByRole("button", (name: 'Submit']).click();

await page.getByBgle("link", (name: "Shop")).click();
