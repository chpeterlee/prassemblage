const { AppiumDriver, createDriver } = require('nativescript-dev-appium');

let driver;

async function main() {
  driver = await createDriver();

  // Launch the Calculator app on the Windows machine
  await driver.runApp('Calculator');

  // Wait for the app to load
  await driver.sleep(3000);

  // Tap the "1" button
  const oneButton = await driver.findElementByAccessibilityId('num1Button');
  await oneButton.click();

  // Tap the "plus" button
  const plusButton = await driver.findElementByAccessibilityId('plusButton');
  await plusButton.click();

  // Tap the "1" button again
  await oneButton.click();

  // Tap the "equals" button
  const equalsButton = await driver.findElementByAccessibilityId('equalButton');
  await equalsButton.click();

  // Get the result element and print the result to the console
  const resultElement = await driver.findElementByAccessibilityId('CalculatorResults');
  const result = await resultElement.text();
  console.log(result);

  // Close the driver
  await driver.quit();
}

main();
--


Appium mobile script
Rewrite for windows